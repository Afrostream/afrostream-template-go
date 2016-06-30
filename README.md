# Description

Minimalist go server using heroku

# Golang Install for ubuntu

```
sudo add-apt-repository ppa:ubuntu-lxc/lxd-stable
sudo apt-get update
sudo apt-get install golang
```

install dependency management tool "godep"

```
go get github.com/tools/godep
```

setup .bashrc env vars

```
export GOPATH=$HOME/go
export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
source ~/.bashrc
```

# Create a project base on this template

we want to work in ~/go/src/github.com/afrostream/hello :

```
# create the directory
mkdir -p $GOPATH/src/github.com/hello
cd  $GOPATH/src/github.com/hello
git clone git@github.com:Afrostream/hello.git
# your source code is now in
cd $GOPATH/src/github.com/afrostream/hello
```

# Run dev

```
npm run dev
```

or

```
go run main.go
```

# clean

```
npm run clean
```

or

```
rm -rf dist/
```

# build

```
npm run build
```

executable is in dist/hello

# Run prod

```
npm start
```

or

```
./dist/hello
```
