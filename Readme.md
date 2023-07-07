# Cfs Workspace

This is a workspace for the Cfs implementation.

## Projects

### Cfs

The repository for the Cfs library is located at 

```
./cfs
```

Refer to its documentation for more information.

### Mkcfs

The repository for the Mkfs tool is located at 

```
./mkcfs
```

Refer to its documentation for more information.

### Cfs Cli

The command line interface for interacting with Cfs is located at 

```
./cfs_cli
```

Refer to its documentation for more information.

## Building

First off all, you need to clone the repository and its submodules:

```bash
git clone --recurse-submodules git@github.com:gnussy/cfs_ws.git
```

Also, you should have the rust toolchain installed. You can install it with [rustup](https://rustup.rs/).

```
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

After, build all of the projects with the following command:

```bash
cargo build --workspace --release
```

## Running

The `mkcfs` format tool can be run with the following command:

```bash
cargo run --release --package mkcfs -- --help
cargo run --release --package mkcfs -- cfs.img -b 4096
```

The `cfs_cli` command line interface can be run with the following command:

```bash
cargo run --release --package cfs_cli -- --help
```
