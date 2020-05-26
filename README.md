# Bitcoin transaction size calculator

## 🏃‍♀️ Usage

* [Run it as command line program](#run)
* [Import in other Golang projects](#import)


### Run
Run it as program in the command line

1. [Dowload the binary for your system](https://github.com/tiero/bitcoin-tx-size/releases)
2. Move it to your PATH. eg. `mv btcsize-darwin-amd64 /usr/bin/btcsize`
3. Use it from the commandline
```sh
$ btcsize "<psbt>"
Size: 850 B
Virtual size: 594 vB
```

### Import
Import in other Go projects

```sh
go get -u github.com/tiero/bitcoin-tx-size
```
```go
import "github.com/tiero/bitcoin-tx-size/pkg/calculator"
```

## 🖥 Development

* Clone 
```sh
$ git clone https://github.com/tiero/bitcoin-tx-size
```

* Install
```sh
$ go install ./...
```

* Test 
```sh
$ go test -v ./...
```

* Build the program for Linux
```
$ GOOS=linux GOARCH=amd64 go build -o btcsize-linux-amd64 ./cmd/
```

* Build the program for Mac
```
$ GOOS=darwin GOARCH=amd64 go build -o btcsize-darwin-amd64 ./cmd/
```



