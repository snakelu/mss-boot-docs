# mss-boot document

### install hugo
please install hugo and extended
https://gohugo.io/getting-started/installing/

### download theme
```shell
mkdir themes && cd themes && git clone https://github.com/StefMa/hugo-fresh.git
```

### run hugo server
```shell
hugo server -D
```
### generate pd.go file

#### mac install step

1. install protobuf
```shell
brew install protobuf
```

2. install go plugins
```shell
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
```

3. update your PATH so that the protoc compiler can find the plugins
```shell
export PATH="$PATH:$(go env GOPATH)/bin"
```
