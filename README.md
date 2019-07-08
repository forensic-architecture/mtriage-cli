# mtriage-cli

### NB: currently unstable, in active development, and should not be used in production

##### generate .yaml files for specifying mtriage workflows

mtriage-cli is a command-line application for generating .yaml configuration files for [mtriage](https://github.com/forensic-architecture/mtriage), an application that scrapes and analyses public domain media. mtriage-cli is developed by [Forensic Architecture](https://forensic-architecture.org), and is intended for use by open source research agencies, journalists, and activists.

## development
mtriage-cli is currently in active development. It is written in Go, and is based on the Gocui package.

mtriage-cli comes packaged as binary, or can be built locally (requiring the depencies lisrted below). The binary must first it must be added to the system PATH, and then run `mgen` in the base directory of mtriage.

### dependencies
- [Go](https://golang.org/doc/install)
- [gocui](https://github.com/jroimartin/gocui)
- [go-yaml](https://github.com/go-yaml/yaml)


### building locally
You can build the mtriage-cli image locally by running:
```bash
go build -o bin/mgen
