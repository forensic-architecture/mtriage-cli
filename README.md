# mtriage-cli

### NB: currently unstable, in active development, and should not be used in production

#### generate .yaml files for specifying mtriage workflows

mtriage-cli is a command-line application for generating .yaml configuration files for [mtriage](https://github.com/forensic-architecture/mtriage), an application that scrapes and analyses public domain media. mtriage-cli is developed by [Forensic Architecture](https://forensic-architecture.org), and is intended for use by open source research agencies, journalists, and activists.

## development
mtriage-cli is currently in active development. It is written in Go, and is based on the Gocui package.

mtriage-cli comes packaged as binary, or can be built locally (requiring the depencies listed below). The binary must first be added to the system PATH, and then launced by running `mgen` in the base directory of mtriage.

### dependencies
- [Go](https://golang.org/doc/install)
- [gocui](https://github.com/jroimartin/gocui) - install with `go get github.com/jroimartin/gocui`
- [go-yaml](https://github.com/go-yaml/yaml) - install with `go get gopkg.in/yaml.v2`


### building locally
You can build the mtriage-cli executable locally by running:
```bash
go build -o bin/mgen
