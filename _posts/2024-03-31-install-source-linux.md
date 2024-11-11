---
layout: post
title:  "Installing Software from Source on Fedora"
date:   2024-03-31 10:26:24 -0500
---

There might be times where you will need to install an application from source, meaning to take the application source code and compile it into a working application. 
 
This can be because of the fact that:
 
* No pre-compiled binary or application package is available.  
* You have specific dependency requirements that are not available in the pre-compiled package.  
* The available pre-compiled application is out of date and you need a specific version.  
 
In these cases you will need to install the software from the command line, using the source files provided by the application developers or maintainers. 
 
## Before you start 
 
To install an application from source, you will need to have:
 
* A way to extract the source file archive. This is usually an application such as `tar` or `gzip`.  
* A build tool and a compiler, such as `make`.  
 
These tools are generally installed by default on a modern Fedora system. You can verify that they are available by typing in `make`, `tar`, and `gzip` from the command line. You will see instructions on how to use the application if it is available. If the application is not available you will get an error along with instructions on how to install.
 
## How to install from source 
 
To install from source, you will need to do the following:
 
* Download the application archive file to your computer. The default location is the Downloads folder, but you might be able to choose a location during the download process.  
* Extract the files from the downloaded archive. The command you use will depend on the application package.  
* Carefully read any instructions that came with your download. These instructions might also be available on the website you downloaded the file from. These instructions will tell you what you need to do to install the application.  
* Follow the commands given in the README (or other installation instructions) to configure, build, compile, and install the application.  
 
### Download the application archive to your computer
The default download location is  your Downloads folder. From the command line the location is `/home/username/Downloads` (note the capital D in Downloads). 
 
### Extract the files from the archive
Most applications require many files or even directories, packaged together into an archive. The most common archives are "tarballs," with the files packaged by using the `tar` (tape archive) command. These will have a `.tar` file extension. 
 
In some cases the files will use a variation of the Zip archive format, such as `.zip` or `.gz`.  Depending on the size of the download the application developer might use both `tar` and `gzip` together, so that the file will have a `.tar.gz` extension.
 
To extract files from a `.tar` archive:
`````
$ tar -xf archive.tar
`````

`-xf` means to e**x**tract the **f**iles from the `tar` archive.
 
To extract files from a `tar.gz` archive:
`````
$ tar -zxf archive.tar.gz
`````

`-zxf` means to un**z**ip the archive, and e**x**tract the **f**iles from the `tar` archive.
 
To extract files from a `.gz` archive:
`````
$ gzip -d archive.gz
`````

`-d` means to **d**ecompress the archive, which extracts the files.
 
You can also use `gunzip`, which is an alias for `gzip -d`. 
`````
$ gunzip archive.gz 
`````

To extract files from a `.zip` archive:
`````
$ unzip archive.zip
`````

Use the `man` command to learn more about `tar`, `gzip`, and `unzip`: `man tar`, `man gzip`, or `man unzip`. You can also find their `man` pages online: https://linux.die.net/man/[Linux man pages]. Search for the command you want to look up. 
 
### Carefully read any instructions that came with your download
When you extract the archive it will leave you with a directory with the same or similar name. You can now change into that directory to find the installation instructions that tell you how to configure and build the application.
 
The extracted folder for the application will have a README or some other file that gives instructions on how to install, configure, and manage the application. The README file will have detailed directions on things such as:
 
* Choosing an alternate directory for installation.  
* Setting configuration options for the build.  
* What compile time options to use for different configurations.  
 
NOTE: If no instructions exist on how to configure or build the application, you will need to reach out to the application developers for help. You might also find instructions online from someone else who had a similar issue.
 
### Follow the instructions to configure, build, compile, and install the application
After you understand what options are available, you can install the application. In general you will need to:
 
* Configure the application by using the `configure` command.
* Build and compile the application by using `make`. 
* Install the application by using `make install`. The `make install` command will need to run using `sudo` so it can write to system directories and local directories. 
 
Here is an example of the entire process, from extracting the files from a `.tar.gz` archive to building the application: 

`````
$ tar -zxf archive.tar.gz
$ cd archive/
$ ./configure 
$ make 
$ sudo make install 
`````

Your application is now installed. The README file or the application website will have more information about how to use the application.
 
NOTE: If you get any errors during the configure and build process, carefully read the error messages and follow the instructions on how to resolve them. There can be dependency issues for some applications, meaning that to install application C, you need to have applications A and B installed. Resolving dependency issues can be challenging and you might need to look for help online to help solve the problem.
 
## See also
 
* [GNU Make (build and compile tool) documentation](https://www.gnu.org/software/make/ "GNU Make")  
* [GNU Tar documentation](https://www.gnu.org/software/tar/ "GNU Tar Documentation")
* [GNU Gzip documentation](https://www.gnu.org/software/gzip/ "GNU Gzip Documentation")
