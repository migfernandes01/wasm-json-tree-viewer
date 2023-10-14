# Description

This project was made for a competition where the goal was to build a JSON tree viewer

## File structure

- `/assets` - contains html file, wasm_exec.js, and wasm binary
- `/cmd` - contains all the go exectuable code
  - `/server` - contains the code to start web server and server html file
  - `/wasm` - contains the code used to generate wasm binary

## Commands

- `GOOS=js GOARCH=wasm go build -o ../../assets/main.wasm ` - build wasm binary (run from `/cmd/wasm` directory)
- `go run main.go` - start web server (run from `/cmd/server`)
