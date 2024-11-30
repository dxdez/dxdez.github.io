---
layout: post
title:  "Creating Dynamic URLs with a Basic Directory Walkthrough"
date:   2024-11-29 10:26:24 -0500
---

### Creating Dynamic URLs with a Basic Directory Walkthrough

This example shows the steps in creating a set of dynamic routes in Golang. These routes are based on the present directories within a `sites` folder inside the template directory. When a folder is found, it builds the route based on the name of that folder. For example, if the folder is named `testsite` then it will create a route called `/testsite` which will navigate to the html + resources of that folder. 
  
The purpose of this is so that games can be dynamically added to the LyteCade templates and from there have their routes and resources automatically configured. 
  
The basic structure of the code is below:
```go
func RouteSites() {
        err := filepath.Walk("./web/sites", func(path string, info os.FileInfo, err error) error {
                if err != nil {
                        return err
                }
                if !info.IsDir() {
                        return nil
                }
                fmt.Println(path)
                currentSite := strings.TrimPrefix(path, "./web/sites")
                if currentSite == "" {
                        return nil
                }
                http.HandleFunc(fmt.Sprintf("/%s", currentSite), func(w http.ResponseWriter, r *http.Request) {
                        pages.HandleGamePage(w, r, currentSite)
                })
                http.Handle("/" + currentSite + "/assets/", pages.HandleGameFolder(currentSite, path, "assets"))
                http.Handle("/" + currentSite + "/src/", pages.HandleGameFolder(currentSite, path, "src"))

                return nil
        })
        if err != nil {
                fmt.Println("Error registering game server:", err)
        }
}
```

The game folder function for pages returns a basic file server URL which can be used for the HTTP handle function:
```go
func HandleGameFolder(siteName, originalPath, resourceFolder string) http.Handler {
        filePrefix := ("/" + siteName + "/" + resourceFolder)
        fileServer := http.StripPrefix(filePrefix, http.FileServer(http.Dir(filepath.Join(originalPath, resourceFolder))))
        return fileServer
}
```

This is still a work in progress however the basic handling of this functionality is complete. The next steps will involve refining the prefix trimming so that instead of the route being `/web/sites/testname` it can instead be simply `/testname`
