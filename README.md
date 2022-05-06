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


TODO: add: crossbeam, num, nalgebra, chrono, clap, log, env_logger, mockall

# no_std
## General
Most of the listed crates such as the serde, serde_derive, tap, ... may also be useful in std environment.
- [heapless](https://crates.io/crates/heapless): _Static friendly data structures that don't require dynamic memory allocation._ [#static, #no-heap] ![crates.io](https://img.shields.io/crates/v/heapless.svg)
- [tap](https://crates.io/crates/tap): _Provides extension methods on all types that allow transparent, temporary, inspection/mutation (tapping), transformation (piping), or type conversion._ [#tap_some #tap, #functional, #tap_ok, #pipe] ![crates.io](https://img.shields.io/crates/v/tap.svg)
- [serde](https://crates.io/crates/serde): _Serde is a framework for serializing and deserializing Rust data structures efficiently and generically._ [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde.svg)
- [serde_derive](https://crates.io/crates/serde_derive): _Serde is a framework for serializing and deserializing Rust data structures efficiently and generically._ [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde_derive.svg)
- [snafu](https://crates.io/crates/snafu): _SNAFU is a library to easily assign underlying errors into domain-specific errors while adding context._ [#no_std, #ergonomic, #library, #error] ![crates.io](https://img.shields.io/crates/v/snafu.svg)
- [tap](https://crates.io/crates/once_cell): _``` once_cell ``` provides two new cell-like types,  ``` unsync::OnceCell ``` and ``` sync::OnceCell ```. _ [#static, #lazy] ![crates.io](https://img.shields.io/crates/v/once_cell.svg)
- [rand](https://crates.io/crates/rand): _A Rust library for random number generation._ [#rng, #random] ![crates.io](https://img.shields.io/crates/v/rand.svg)
- [itertools](https://crates.io/crates/itertools): _Extra iterator adaptors, functions and macros._ [#zip, #product, #group-by, #iterator, #data-structure] ![crates.io](https://img.shields.io/crates/v/itertools.svg)

## Platform
### Embedded
### Wasm

# std
## General
- [Rayon](https://crates.io/crates/rayon): _Rayon is a data-parallelism library for Rust._ [#performance, #thread, #parallel, #join, #concurrency] ![crates.io](https://img.shields.io/crates/v/rayon.svg)

## Libraries
- [thiserror](https://crates.io/crates/thiserror): _Provides a convenient derive macro for the standard library's ``` std::error::Error trait ```._ ![crates.io](https://img.shields.io/crates/v/thiserror.svg)

## Applications
- [Anyhow](https://crates.io/crates/Anyhow): _Provides ``` anyhow::Error ```, a trait object based error type for easy idiomatic error handling in Rust applications._ ![crates.io](https://img.shields.io/crates/v/Anyhow.svg)
- [tokio](https://crates.io/crates/tokio): _A runtime for writing reliable, asynchronous, and slim applications with the Rust programming language._ [#async, #futures, #io, #non-blocking] ![crates.io](https://img.shields.io/crates/v/tokio.svg)
- [tracing](https://crates.io/crates/tracing): _tracing is a framework for instrumenting Rust programs to collect structured, event-based diagnostic information._ [#logging, #tracing, #metrics, #async] ![crates.io](https://img.shields.io/crates/v/tracing.svg)
- [fs-err](https://crates.io/crates/fs-err): _``` fs-err ``` is a drop-in replacement for std::fs that provides more helpful messages on errors._ [#logging, #tracing, #metrics, #async] ![crates.io](https://img.shields.io/crates/v/fs-err.svg)

## Domain
### Gui

### Backend
- [reqwest](https://crates.io/crates/reqwest): _An ergonomic, batteries-included HTTP Client for Rust._ [#client, #request, #http] ![crates.io](https://img.shields.io/crates/v/reqwest.svg)

# Build

- bindgen

# Test
- [insta](https://crates.io/crates/insta): _Snapshots tests (also sometimes called approval tests) are tests that assert values against a reference value (the snapshot)._ [#testing, #snapshot, #approval, #jest] ![crates.io](https://img.shields.io/crates/v/insta.svg)
- [Fake](https://crates.io/crates/Fake): _A Rust library for generating fake data._ [#random, #data, #generator, #faker] ![crates.io](https://img.shields.io/crates/v/Fake.svg)
- [wiremock](https://crates.io/crates/wiremock): _wiremock provides HTTP mocking to perform black-box testing of Rust applications that interact with third-party APIs._ [#mock, #black-box, #http, #mocking, #test] ![crates.io](https://img.shields.io/crates/v/wiremock.svg)

# Macro
- [syn](https://crates.io/crates/syn): _Syn is a parsing library for parsing a stream of Rust tokens into a syntax tree of Rust source code._ ![crates.io](https://img.shields.io/crates/v/syn.svg)
- [quote](https://crates.io/crates/quote): _This crate provides the quote! macro for turning Rust syntax tree data structures into tokens of source code._ ![crates.io](https://img.shields.io/crates/v/quote.svg)
- [proc-macro2](https://crates.io/crates/proc-macro2): _A wrapper around the procedural macro API of the compiler's proc_macro crate._ [#macros] ![crates.io](https://img.shields.io/crates/v/proc-macro2.svg)
- [paste](https://crates.io/crates/paste): _Provides a flexible way to paste together identifiers in a macro, including using pasted identifiers to define new items._ ![crates.io](https://img.shields.io/crates/v/paste.svg)


# Cargo


# Other resources
- [Awesome Rust Embedded](https://github.com/rust-embedded/awesome-embedded-rust) *This is a curated list of resources related to embedded and low-level programming in the programming language Rust, including a list of useful crates.*

