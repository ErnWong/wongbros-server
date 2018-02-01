A small collection of scripts to help running my private [OpenRCT2](https://openrct2.website/) server. Emphasis on the word "private".

The scripts here checks for, and if necessary, updates the OpenRCT2 binaries (similar to the [OpenRCT2 Launcher](https://github.com/LRFLEW/OpenRCT2Launcher)).

## Installing

[Node.js](https://nodejs.org/en/) is required. After cloning/downloading this repo, install the required npm dependencies:

```sh
npm install
```

Linux machines will also need to install [OpenRCT2 Dependencies](https://github.com/OpenRCT2/OpenRCT2/wiki/Building-OpenRCT2-on-Linux#required-packages-general). If you're on Ubuntu, an example install script is provided for convenience:

```sh
./install-deps.sh
```

## Running

```sh
./run [options]
```

Options:

- By default, `./run` checks updates for and downloads **Linux** binaries, and runs the server.
- `--update`: Only check for and download updates. Don't run the server.
- `--windows`: Check updates for and download **Windows** binaries instead.

OpenRCT2 will look for OpenRCT2 user data at `./data`. Downloaded binaries will live inside `./bin`.
