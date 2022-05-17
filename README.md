# Must know rust crates
This repository contains a list of the most common must know crates in the rust ecosystem. 
It intends to be a short and evolving overview of useful development crates and tools for Rust. For a more exhaustive list, including software written in Rust and all kinds of frameworks, you are probably better served by checking out the [Awesome Rust](https://github.com/rust-unofficial/awesome-rust) list.
The crates are group into no_std, std, build, test, macro, cargo and further which platform and project they are useful for.

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

# no_std
## General
Most of the listed crates such as the serde, serde_derive, tap, ... may also be useful in std environment.
- [heapless](https://crates.io/crates/heapless): _Static friendly data structures that don't require dynamic memory allocation._ [#static, #no-heap] ![crates.io](https://img.shields.io/crates/v/heapless.svg)
- [tap](https://crates.io/crates/tap): _Provides extension methods on all types that allow transparent, temporary, inspection/mutation (tapping), transformation (piping), or type conversion._ [#tap_some #tap, #functional, #tap_ok, #pipe] ![crates.io](https://img.shields.io/crates/v/tap.svg)
- [serde](https://crates.io/crates/serde): _Serde is a framework for serializing and deserializing Rust data structures efficiently and generically._ [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde.svg)
- [serde_derive](https://crates.io/crates/serde_derive): _Serde is a framework for serializing and deserializing Rust data structures efficiently and generically._ [#serialization, #no_std, #serde] ![crates.io](https://img.shields.io/crates/v/serde_derive.svg)
- [snafu](https://crates.io/crates/snafu): _SNAFU is a library to easily assign underlying errors into domain-specific errors while adding context._ [#no_std, #ergonomic, #library, #error] ![crates.io](https://img.shields.io/crates/v/snafu.svg)
- [once_cell](https://crates.io/crates/once_cell): _``` once_cell ``` provides two new cell-like types,  ``` unsync::OnceCell ``` and ``` sync::OnceCell ```._ [#static, #lazy] ![crates.io](https://img.shields.io/crates/v/once_cell.svg)
- [rand](https://crates.io/crates/rand): _A Rust library for random number generation._ [#rng, #random] ![crates.io](https://img.shields.io/crates/v/rand.svg)
- [itertools](https://crates.io/crates/itertools): _Extra iterator adaptors, functions and macros._ [#zip, #product, #group-by, #iterator, #data-structure] ![crates.io](https://img.shields.io/crates/v/itertools.svg)
- [Crossbeam](https://crates.io/crates/Crossbeam): _Provides a set of tools for concurrent programming._ [#garbage, #non-blocking, #rcu #atomic, #lock-free] ![crates.io](https://img.shields.io/crates/v/Crossbeam.svg)
- [nom](https://crates.io/crates/nom): _nom is a parser combinators library written in Rust._ [#parser, #parsing, #streaming, #bit, #parser-combinators] ![crates.io](https://img.shields.io/crates/v/nom.svg)
- [num](https://crates.io/crates/num): _A collection of numeric types and traits for Rust._ [#mathematics, #numerics, #bignum] ![crates.io](https://img.shields.io/crates/v/num.svg)
- [nalgebra](https://crates.io/crates/nalgebra): _Linear algebra library for the Rust programming language._ [#math, #algebra, #linear, #matrix, #vector] ![crates.io](https://img.shields.io/crates/v/nalgebra.svg)
- [Chrono](https://crates.io/crates/chrono): _It aims to be a feature-complete superset of the time library._ [#time, #date, #calendar] ![crates.io](https://img.shields.io/crates/v/chrono.svg)
- [lazy_static](https://crates.io/crates/lazy_static): _A macro for declaring lazily evaluated statics in Rust._ [#macro, #static, #lazy] ![crates.io](https://img.shields.io/crates/v/lazy_static.svg)
- [time](https://crates.io/crates/time): _ Date and time library. Fully interoperable with the standard library._ [#time, #date, #calendar, #duration] ![crates.io](https://img.shields.io/crates/v/time.svg)

## Platform
### Embedded
- [Awesome Rust Embedded](https://github.com/rust-embedded/awesome-embedded-rust) *This is a curated list of resources related to embedded and low-level programming in the programming language Rust, including a list of useful crates.*
- [embedded-hal](https://crates.io/crates/embedded-hal): _A Hardware Abstraction Layer (HAL) for embedded systems._ [#io, #hal] ![crates.io](https://img.shields.io/crates/v/embedded-hal.svg)
- [svd2rust](https://crates.io/crates/svd2rust): _Generate Rust register maps (structs) from SVD files._ [#map, #embedded, #generator, #register, #svd] ![crates.io](https://img.shields.io/crates/v/svd2rust.svg)
- [defmt](https://crates.io/crates/defmt): _defmt ("de format", short for "deferred formatting") is a highly efficient logging framework that targets resource-constrained devices, like microcontrollers._ [#logging, #logger, #formatter, #formatting, #knurling] ![crates.io](https://img.shields.io/crates/v/defmt.svg)
- [cargo-flash](https://crates.io/crates/cargo-flash): _This crate provides a cargo subcommand to flash ELF binaries onto ARM chips._ [#embedded] ![crates.io](https://img.shields.io/crates/v/cargo-flash.svg)
- [cargo-embed](https://crates.io/crates/cargo-embed): _This crate provides a cargo subcommand to work with embedded targets._ [#embedded] ![crates.io](https://img.shields.io/crates/v/cargo-embed.svg)
- [embedded-hal-mock](https://crates.io/crates/embedded-hal-mock): _This is a collection of types that implement the embedded-hal traits._ [#io, #i2c, #hal, #delay, #spi] ![crates.io](https://img.shields.io/crates/v/embedded-hal-mock.svg)
### Wasm
- [Rust Wasm Book](https://rustwasm.github.io/docs/book/introduction.html) *This small book describes how to use Rust and WebAssembly together.*
- [wasm-pack](https://crates.io/crates/wasm-pack): _This tool seeks to be a one-stop shop for building and working with rust- generated WebAssembly that you would like to interop with JavaScript, in the browser or with Node.js._ ![crates.io](https://img.shields.io/crates/v/wasm-pack.svg)
- [wasm-bindgen-futures](https://crates.io/crates/wasm-bindgen-futures): _This crate bridges the gap between a Rust Future and a JavaScript Promise._ ![crates.io](https://img.shields.io/crates/v/wasm-bindgen-futures.svg)
- [js-sys](https://crates.io/crates/js-sys): _Raw bindings to JS global APIs for projects using wasm-bindgen._ ![crates.io](https://img.shields.io/crates/v/js-sys.svg)
- [web-sys](https://crates.io/crates/web-sys): _Raw bindings to Web APIs for projects using wasm-bindgen._ ![crates.io](https://img.shields.io/crates/v/web-sys.svg)

# std
## General
Also check out the [no_std general](#general) section as most of the crates in no_std general will also be useful in the std environment.

- [Rayon](https://crates.io/crates/rayon): _Rayon is a data-parallelism library for Rust._ [#performance, #thread, #parallel, #join, #concurrency] ![crates.io](https://img.shields.io/crates/v/rayon.svg)
- [camino](https://crates.io/crates/camino): _This repository contains the source code for camino, an extension of the std::path module that adds new Utf8PathBuf and Utf8Path types._ [#unicode, #filesystem, #utf8, #paths] ![crates.io](https://img.shields.io/crates/v/camino.svg)
- [strum](https://crates.io/crates/strum): _Strum is a set of macros and traits for working with enums and strings easier in Rust._ [#macros, #string, #enum, #proc-macros] ![crates.io](https://img.shields.io/crates/v/strum.svg)

## Libraries
- [thiserror](https://crates.io/crates/thiserror): _Provides a convenient derive macro for the standard library's ``` std::error::Error trait ```._ ![crates.io](https://img.shields.io/crates/v/thiserror.svg)
- [log](https://crates.io/crates/log): _A Rust library providing a lightweight logging facade._ [#logging] ![crates.io](https://img.shields.io/crates/v/log.svg)

## Applications
- [Anyhow](https://crates.io/crates/Anyhow): _Provides ``` anyhow::Error ```, a trait object based error type for easy idiomatic error handling in Rust applications._ ![crates.io](https://img.shields.io/crates/v/Anyhow.svg)
- [color-eyre](https://crates.io/crates/color-eyre): _An error report handler for panics and the eyre crate for colorful, consistent, and well formatted error reports for all kinds of errors._ ![crates.io](https://img.shields.io/crates/v/color-eyre.svg)
- [tokio](https://crates.io/crates/tokio): _A runtime for writing reliable, asynchronous, and slim applications with the Rust programming language._ [#async, #futures, #io, #non-blocking] ![crates.io](https://img.shields.io/crates/v/tokio.svg)
- [tracing](https://crates.io/crates/tracing): _tracing is a framework for instrumenting Rust programs to collect structured, event-based diagnostic information._ [#logging, #tracing, #metrics, #async] ![crates.io](https://img.shields.io/crates/v/tracing.svg)
- [fs-err](https://crates.io/crates/fs-err): _``` fs-err ``` is a drop-in replacement for std::fs that provides more helpful messages on errors._ [#logging, #tracing, #metrics, #async] ![crates.io](https://img.shields.io/crates/v/fs-err.svg)
- [clap](https://crates.io/crates/clap): _Command Line Argument Parser for Rust._ [#parser, #argument, #cli, #parse, #arg] ![crates.io](https://img.shields.io/crates/v/clap.svg)
- [env_logger](https://crates.io/crates/env_logger): _Implements a logger that can be configured via environment variables._ [#log, #logging, #logger] ![crates.io](https://img.shields.io/crates/v/env_logger.svg)

## Domain
### Backend
- [reqwest](https://crates.io/crates/reqwest): _An ergonomic, batteries-included HTTP Client for Rust._ [#client, #request, #http] ![crates.io](https://img.shields.io/crates/v/reqwest.svg)
- [hyper](https://crates.io/crates/hyper): _A fast and correct HTTP implementation for Rust._ [#hyper, #http, #hyperium] ![crates.io](https://img.shields.io/crates/v/hyper.svg)
- [H2](https://crates.io/crates/h2): _A Tokio aware, HTTP/2 client & server implementation for Rust._ [#http, #async, #non-blocking] ![crates.io](https://img.shields.io/crates/v/h2.svg)
### Gui
### Game

# Build
- [bindgen](https://crates.io/crates/bindgen): _bindgen automatically generates Rust FFI bindings to C (and some C++) libraries._ [#bindings, #ffi, #code-generation] ![crates.io](https://img.shields.io/crates/v/bindgen.svg)

# Test
- [insta](https://crates.io/crates/insta): _Snapshots tests (also sometimes called approval tests) are tests that assert values against a reference value (the snapshot)._ [#testing, #snapshot, #approval, #jest] ![crates.io](https://img.shields.io/crates/v/insta.svg)
- [Fake](https://crates.io/crates/Fake): _A Rust library for generating fake data._ [#random, #data, #generator, #faker] ![crates.io](https://img.shields.io/crates/v/Fake.svg)
- [wiremock](https://crates.io/crates/wiremock): _wiremock provides HTTP mocking to perform black-box testing of Rust applications that interact with third-party APIs._ [#mock, #black-box, #http, #mocking, #test] ![crates.io](https://img.shields.io/crates/v/wiremock.svg)
- [Mockall](https://crates.io/crates/Mockall): _A powerful mock object library for Rust._ [#testing, #mock, #mocking] ![crates.io](https://img.shields.io/crates/v/Mockall.svg)
- [criterion](https://crates.io/crates/criterion): _Criterion.rs helps you write fast code by detecting and measuring performance improvements or regressions, even small ones, quickly and accurately._ [#benchmark, #criterion] ![crates.io](https://img.shields.io/crates/v/criterion.svg)


# Macro
- [syn](https://crates.io/crates/syn): _Syn is a parsing library for parsing a stream of Rust tokens into a syntax tree of Rust source code._ ![crates.io](https://img.shields.io/crates/v/syn.svg)
- [quote](https://crates.io/crates/quote): _This crate provides the quote! macro for turning Rust syntax tree data structures into tokens of source code._ ![crates.io](https://img.shields.io/crates/v/quote.svg)
- [proc-macro2](https://crates.io/crates/proc-macro2): _A wrapper around the procedural macro API of the compiler's proc_macro crate._ [#macros] ![crates.io](https://img.shields.io/crates/v/proc-macro2.svg)
- [paste](https://crates.io/crates/paste): _Provides a flexible way to paste together identifiers in a macro, including using pasted identifiers to define new items._ ![crates.io](https://img.shields.io/crates/v/paste.svg)


# Cargo
- [cargo-edit](https://crates.io/crates/cargo-edit): _This tool extends Cargo to allow you to add, remove, and upgrade dependencies by modifying your Cargo.toml file from the command line._ ![crates.io](https://img.shields.io/crates/v/cargo-edit.svg)
- [cargo-outdated](https://crates.io/crates/cargo-outdated): _A cargo subcommand for displaying when Rust dependencies are out of date._ ![crates.io](https://img.shields.io/crates/v/cargo-outdated.svg)
- [cargo-update](https://crates.io/crates/cargo-update): _A cargo subcommand for checking and applying updates to installed executables._ ![crates.io](https://img.shields.io/crates/v/cargo-update.svg)
- [cargo-expand](https://crates.io/crates/cargo-expand): _Once installed, the following command prints out the result of macro expansion and ``` #[derive] ``` expansion applied to the current crate._ ![crates.io](https://img.shields.io/crates/v/cargo-expand.svg)
