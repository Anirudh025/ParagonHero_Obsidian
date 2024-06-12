#rust #code
## New Cargo
``` terminal
cargo new {cargo_name}
cargo {cargo_name}
```

## Cargo TOMLs
#TOML, Tom's Obvious Minimal Language
 Cargo TOML formats look somewhat like this
 ``` TOML
[package]
name = "{cargo name}"
version = "0.1.0"
edition = "2021"

# See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html

[dependencies]
 
```
The first line, `[package]`, is a section heading that indicates that the following statements are configuring a package. As we add more information to this file, we’ll add other sections. The next three lines set the configuration information Cargo needs to compile your program: the name, the version, and the edition of Rust to use. The last line, `[dependencies]`, is the start of a section for you to list any of your project’s dependencies. In Rust, packages of code are referred to as [_crates_](crates.md).

## Cargo build/run
Cargos need to be built to use properly and create executables
``` Terminal
cargo build
```

The result looks like
``` terminal
```
