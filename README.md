# Go for JS Dev
## Setup GO
- [Download and install GO](https://go.dev/dl/)
- If you're installing Go for the first time, start at the section `Installing Go From Scratch`
## Installing Go
### Installing Go From Scratch
#### Download Go
- Visit [golang.org/dl](https://golang.org/dl) 
- Select the download package for your operating system
- Once the installation package is downloaded, double click on that package to kick off installation. 

#### Verify Installation
When the installation wizard is complete, open up a terminal window and verify Go is installed with the following commands: 

```bash
which go
=> /usr/local/go/bin/go

go version
=> go version go1.16 darwin/amd64
```

#### Modify Your PATH 
- Go checks for a certain environment variable, `GOPATH` when executing a Go program. We need to update our bash_profile to help Go find where our files will live.
- In a code editor, open up your `.bash_profile` which should be located in your home directory. 
- Add the following lines to the bottom of the file (or wherever you export your PATH environment variables)

```bash
export GOPATH=$HOME/go
export GOBIN=$GOPATH/bin
export PATH=$PATH:$GOBIN
```

### Upgrading to Go Latest
Verify you do have Go installed in the first place:

```bash
go version 
=> go version go1.16 darwin/amd64
```

Uninstall Go

```bash
sudo rm -rf /usr/local/go
```

Verify Go was uninstalled

```bash
go version
=> -bash: go: command not found
```

Visit [golang.org/dl](https://golang.org/dl) to install the latest Go.
