# Must know rust crates
This repository contains a list of the most common must know crates in the rust ecosystem. 
The crates are group into no_std, std, build, test, macro and cargo and further which platform and project they are useful for. 

# Table of contents
- [no_std](#no_std)
- - [General](#general)
- - [Platform](#platform)
- - - [Embedded](#embedded)
- - - [Wasm](#wasm)

- [std](#std)
- - [General](#general)
- - [Libraries](#libraries)
- - [Applications](#applications)

- - [Domain](#domain)
- - - [Gui](#gui)
- - - [Backend](#backend)
- [Build](#build)
- [Test](#test)
- [Macro](#macro)
- [Cargo](#cargo)
- [Other resources](#other-resources)

# no_std
## General
Most of the listed crates such as the serde, serde_derive, tap, ... may also be useful in std environment.
- [heapless](https://crates.io/crates/heapless): *Static friendly data structures that don't require dynamic memory allocation.* [#static, #no-heap] ![crates.io](https://img.shields.io/crates/v/heapless.svg)
- [tap](https://crates.io/crates/tap): *Provides extension methods on all types that allow transparent, temporary, inspection/mutation (tapping), transformation (piping), or type conversion.* [#tap_some #tap, #functional, #tap_ok, #pipe] ![crates.io](https://img.shields.io/crates/v/tap.svg)
- [serde](https://crates.io/crates/serde): *Serde is a framework for serializing and deserializing Rust data structures efficiently and generically.* [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde.svg)
- [serde_derive](https://crates.io/crates/serde_derive): *Serde is a framework for serializing and deserializing Rust data structures efficiently and generically.* [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde_derive.svg)
- [snafu](https://crates.io/crates/snafu): *SNAFU is a library to easily assign underlying errors into domain-specific errors while adding context.* [#no_std, #ergonomic, #library, #error] ![crates.io](https://img.shields.io/crates/v/snafu.svg)

## Platform
### Embedded
### Wasm

# std
## General
- [Rayon](https://crates.io/crates/rayon): *Rayon is a data-parallelism library for Rust.* [#performance, #thread, #parallel, #join, #concurrency] ![crates.io](https://img.shields.io/crates/v/rayon.svg)

## Libraries
- [thiserror](https://crates.io/crates/thiserror): *Provides a convenient derive macro for the standard library's std::error::Error trait.* ![crates.io](https://img.shields.io/crates/v/thiserror.svg)
## Applications
- [Anyhow](https://crates.io/crates/Anyhow): *Provides ``` anyhow::Error ```, a trait object based error type for easy idiomatic error handling in Rust applications.* ![crates.io](https://img.shields.io/crates/v/Anyhow.svg)

## Domain
### Gui

# Build

- bindgen

# Test

# Macro
- [syn](https://crates.io/crates/syn): *Syn is a parsing library for parsing a stream of Rust tokens into a syntax tree of Rust source code.* ![crates.io](https://img.shields.io/crates/v/syn.svg)
- [quote](https://crates.io/crates/quote): *This crate provides the quote! macro for turning Rust syntax tree data structures into tokens of source code.* ![crates.io](https://img.shields.io/crates/v/quote.svg)
- [proc-macro2](https://crates.io/crates/proc-macro2): *A wrapper around the procedural macro API of the compiler's proc_macro crate.* [#macros] ![crates.io](https://img.shields.io/crates/v/proc-macro2.svg)

# Cargo


# Other resources
- [Awesome Rust Embedded](https://github.com/rust-embedded/awesome-embedded-rust) *This is a curated list of resources related to embedded and low-level programming in the programming language Rust, including a list of useful crates.*

