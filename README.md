# onlineconf

Go package `onlineconf` reads configuration files generated by OnlineConf.

## Example

Read parameters from a module:
```go
module := onlineconf.GetModule("module")
s := module.GetString("/my/parameter", "default value")
i := module.GetInt("/my/parameter", 300)
```

Reading parameters from the module `"TREE"` can be simpler:
```go
s := onlineconf.GetString("/my/parameter", "default value")
i := onlineconf.GetInt("/my/parameter", 300)
```
