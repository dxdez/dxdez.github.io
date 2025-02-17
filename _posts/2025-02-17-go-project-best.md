---
layout: post
title:  "Go Project Setup Best Practices"
date:   2025-02-17 10:01:21 -0500
---

When starting a professional Go project, setting up the right folder structure and adhering to best practices for maintaining packages and repositories will ensure long-term scalability and ease of development. Below are best practices for structuring your Go project, publishing it to `pkg.go.dev`, and maintaining it on GitHub.

### Folder Structure for Go Projects

A clear, consistent folder structure is crucial in Go projects. While Go doesn’t enforce a specific directory structure, there are widely accepted conventions that can be followed for clarity and maintainability.

Here is a typical structure for a Go project:

```
/my-go-project
|-- /cmd
|   |-- /myapp
|       |-- main.go
|
|-- /pkg
|   |-- mypackage.go
|
|-- /internal
|   |-- myinternalpackage.go
|
|-- /api
|   |-- myapi.proto
|
|-- /scripts
|   |-- setup.sh
|
|-- /web
|   |-- /static
|   |-- /templates
|
|-- /docs
|   |-- README.md
|-- /test
|   |-- mypackage_test.go
|-- go.mod
|-- go.sum
```

### Key Folders and Their Purpose

- **cmd/**: Contains the entry point for your application. A Go project can have one or more executable applications. Each one should have its own subdirectory under `cmd/`. For example, if you’re building a CLI tool called `myapp`, you would place the `main.go` file under `cmd/myapp/main.go`. This allows you to organize your various executables independently.
  
- **pkg/**: This folder is used for reusable libraries and packages that can be imported by other projects or applications. Anything placed in the `pkg/` directory should be intended for public use, ideally serving as core business logic, utility functions, or shared components.

- **internal/**: This directory contains packages that are private to the project and cannot be imported outside of it. Go enforces the rule that anything in `internal/` can only be imported by the project it belongs to, providing a mechanism for enforcing encapsulation and preventing external dependencies.

- **api/**: If your project includes any API definitions (such as gRPC or REST API specifications), they should reside here. For gRPC projects, this is typically where `.proto` files are stored.

- **web/**: Contains static assets like HTML, CSS, JavaScript, and templates if your Go project is serving a web interface.

- **scripts/**: If there are any scripts needed to set up, build, or deploy your project (such as deployment scripts or automation tools), place them here.

- **test/**: This folder contains all your test files. Go encourages testing through its built-in `testing` package. Tests for each package should ideally be stored alongside the code they test, but this directory can also house integration or other tests.

### Go Module Setup

Every Go project should use Go modules, which are the official dependency management system in Go. It allows the project to manage versions and dependencies easily. To initialize a Go module:

1. Run `go mod init my-go-project` in the root of your project.
2. As you develop, run `go get` to install dependencies. Go automatically updates your `go.mod` and `go.sum` files to track those dependencies.

### Best Practices for Go Code

- **Organize your code logically**: Group similar functionality together. This makes your project easier to navigate and understand. For example, if you’re working on a file management app, group file handling functions and logic within the `pkg/file` directory.

- **Use Go idioms**: Follow Go’s idiomatic practices. This includes using short variable names (e.g., `err` for errors), structuring functions properly, and following Go’s style guidelines (e.g., avoiding unnecessary semicolons, using indentation for clarity).

- **Write tests**: Use the built-in `testing` package for writing unit tests and coverage. Go encourages simplicity, so keeping tests alongside code is common.

- **Use interfaces**: Go’s interface system is powerful. Where appropriate, use interfaces to define behavior that can be easily mocked or tested in isolation.

### Publishing to pkg.go.dev

Once you have built a reusable Go package, you may want to publish it to `pkg.go.dev`, which makes it accessible to other developers. Here's how you can publish your package:

1. **Tagging the release**: Tag your project with a version number using Git. This is important for Go module versioning.
    ```bash
    git tag v1.0.0
    git push origin v1.0.0
    ```

2. **Make your code public**: Go modules rely on GitHub repositories (or any other public Git repository). Your repository needs to be publicly accessible for it to be indexed by `pkg.go.dev`.

3. **Submit to pkg.go.dev**: Once your code is tagged and public, go to [pkg.go.dev](https://pkg.go.dev) and follow the steps to link your GitHub repository. You can also add a `go.sum` file to ensure consistency across builds.

4. **Documentation**: Your package documentation should be thorough and clear. Ensure that your package has a README file with installation instructions, examples, and usage details. The documentation will be shown on `pkg.go.dev`.

5. **Use `GoDoc` comments**: The GoDoc tool automatically generates documentation from comments in your Go code. Make sure to use GoDoc-style comments on all exported functions, types, and variables.

### Best Practices for GitHub Repositories

Proper maintenance of your GitHub repository is just as important as the code itself. Here are some best practices:

1. **Include a README**: Provide a clear and informative README file at the root of the repository. It should explain the purpose of the project, how to install and use it, and any necessary setup instructions.

2. **License your code**: Include an open-source license in your project. Common licenses include MIT, Apache 2.0, or GPL-3.0. Add a `LICENSE` file to your repository.

3. **Version Control**: Use Git tags to track releases and maintain semantic versioning (e.g., `v1.0.0`, `v1.1.0`). This helps users of your package to know which versions are stable and appropriate to use.

4. **CI/CD**: Set up continuous integration and deployment (CI/CD) pipelines to automatically test your code when changes are pushed to the repository. GitHub Actions, Travis CI, or CircleCI can be integrated to automate testing and building.

5. **Issues and Pull Requests**: Use GitHub’s issue tracker to handle bugs, features, and requests. Ensure that pull requests follow a consistent format and are reviewed before merging into the main branch.

6. **Semantic Commit Messages**: Follow a standard format for commit messages, such as the [Conventional Commits](https://www.conventionalcommits.org/) style. This makes it easier to track changes and automatically generate changelogs.

### Resources for Further Reading

1. **The Go Programming Language** – *The definitive guide to Go programming by Alan A. A. Donovan and Brian W. Kernighan*  
   [Link to book](https://www.oreilly.com/library/view/the-go-programming/9780134190440/)

2. **Go Wiki** – *Go’s official documentation and guidelines*  
   [Go Wiki on GitHub](https://github.com/golang/go/wiki)

3. **GoDoc** – *Go’s official documentation generator*  
   [GoDoc](https://pkg.go.dev/golang.org/x/tools/cmd/godoc)

4. **Go Modules** – *Understanding Go modules and dependency management*  
   [Go Modules Documentation](https://blog.golang.org/using-go-modules)

5. **Effective Go** – *Best practices for Go development*  
   [Effective Go](https://golang.org/doc/effective_go.html)

6. **Go Conventions** – *Go language idioms and best practices*  
   [Go Wiki on Idioms](https://github.com/golang/go/wiki/CodeReviewComments)

By following these best practices and utilizing the resources provided, you will be able to set up a Go project that is well-organized, easy to maintain, and ready for collaboration.
