#programmingParadigms #pwr

[[cargo]] is a tool that makes compiling a rust program easier, it also is responsible for installing, updating and publishing programs and libraries written in rust.

## How to make it work
To make it work you need a basic setup:
```
src/lib.rs or src/main.rs
Cargo.toml
```

In `Cargo.toml` we write information on your program/library like name, author, setting, dependencies and more! The more advance `Cargo.toml` look like this:

```toml
[package]
edition = "2021"
name = "react"
version = "2.0.0"

[build] # Here we sets a flags that will be used in compilation
rustflags = ["-C", "target-cpu=native"] # this means to screw compability and use special asembler

[dependencies]
itertools = "0.11.0" # It is library with a lot of usefull methods implemented for iterators

[target.x86_64-unknown-linux-gnu] # special rules for some target
linker = "/usr/bin/clang" # linker chaged for some that might speed up program
rustflags = ["-Clink-arg=-fuse-ld=lld", "-Clink-arg=-Wl,--no-rosegment"]

[profile.bench] # profile bench means, when we will compile a code for a bench test
debug = true

[profile.release] # this profile is for final version with all of the speed that is possible
lto = "fat"
codegen-units = 1
debug = true
```

## Examples
> [[cargo]] init `name` --lib

it will make a simple directory with a basic structure for a library with some `name`

> [[cargo]] test

it will check if something have changed, compile it, and run tests

> [[cargo]] build 

it will build a library or program in debug mode

