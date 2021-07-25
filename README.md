# Go module
go mod init  github.com/freemanpolys/youtube-golang-module/hello

# Depedencies
```
go mod tidy
```
go mod tidy ensures that the go.mod file matches the source code in the module. It adds any missing module requirements necessary to build the current module's packages and dependencies, and it removes requirements on modules that don't provide any relevant packages. It also adds any missing entries to go.sum and removes unnecessary entries.

# Module replace directive
replace world => ../world

A replace directive replaces the contents of a specific version of a module, or all versions of a module, with contents found elsewhere. The replacement may be specified with either another module path and version, or a platform-specific file path.
