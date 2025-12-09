
## GoQuiet (SIP003)-Linux
env CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-client_linux_amd64 ./cmd/gq-client
env CGO_ENABLED=0 GOOS=linux GOARCH=amd64 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-server_linux_amd64 ./cmd/gq-server

env CGO_ENABLED=0 GOOS=linux GOARCH=386 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-client_linux_386 ./cmd/gq-client
env CGO_ENABLED=0 GOOS=linux GOARCH=386 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-server_linux_386 ./cmd/gq-server

## GoQuiet (SIP003)-WIN
env CGO_ENABLED=0 GOOS=windows GOARCH=amd64 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-client_windows_amd64.exe ./cmd/gq-client
env CGO_ENABLED=0 GOOS=windows GOARCH=amd64 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-server_windows_amd64.exe ./cmd/gq-server

env CGO_ENABLED=0 GOOS=windows GOARCH=386 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-client_windows_386.exe ./cmd/gq-client
env CGO_ENABLED=0 GOOS=windows GOARCH=386 go build -buildvcs=false -ldflags="-s -w" -o ./bin/gq-server_windows_386.exe ./cmd/gq-server
