# httpbox
[![Build Status](https://travis-ci.org/detro/httpbox.svg?branch=master)](https://travis-ci.org/detro/httpbox)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdetro%2Fhttpbox.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdetro%2Fhttpbox?ref=badge_shield)

`httpbox` is a Command line HTTP client that aims to be as feature rich as your shell scripting skills can handle.

**WARNING:** This is me, finally finding the time to learn a bit of Rust and _Rust-best-practices_.
If I'm doing anything wrong, please make sure you yell at me... gently. :)

## Releases

In addition to be able to compile it yourself (see _"How to build"_ section below), releases are also
provided for:

* Linux GNU 32bit and 64bit
* Mac OS X 32bit and 64bit
* Windows GNU 32bit and 64bit

Just check out [/releases](https://github.com/detro/httpbox/releases) for the latest binaries.

## TODO features list

* ~~verbosity control~~
* ~~quiet mode (nothing written on STD_OUT if there are no errors)~~
* ~~help and version flags~~
* ~~meta information for --help coming from Cargo.toml (i.e. single source for binary metadata)~~
* ~~support for all http methods~~
* ~~default output to stdout~~
* ~~able to output to a given file~~
* disable gzip
* provide customer root certificate
* provide headers
* provide User Agent (specialized header)
* provide Cookies (specialized header)
* provide User Agent strings shorthands (i.e. 'macosx-chrome-60' or 'windows-edge')
* multiple concurrent requests to download a file (if supported by target server)
* determine max redirection
* use IPv4 protocol (default)
* use IPv6 protocol
* skip HTTPS certificate verification
* skip download if output file already exists
* proxy configuration
* timeouts (connection / read)
* progress indicator (none, simple, advanced)
* search for mirros (RESEARCH: how do other clients like 'axel' do this?)

## How to build

### Binary executable from [crates.io](https://crates.io/crates/httpbox)

A simple `cargo install` should be all you need to do:

1. Install [rustup](https://www.rustup.rs/)
2. `cargo install httpbox`

### From [GitHub](https://github.com/detro/httpbox) source repository

There is nothing special in how to compile `httpbox` compared to any other Rust binary:

1. Install [rustup](https://www.rustup.rs/)
2. `git clone git@github.com:detro/httpbox.git`
3. `cd httpbox`
4. `cargo build` or `cargo build --release` (for the release artifact, duh!)
5. Binary will be in `target/(debug|release)/httpbox`

## License

[Apache License 2.0](./LICENSE) ([official page](https://www.apache.org/licenses/LICENSE-2.0))


[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdetro%2Fhttpbox.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdetro%2Fhttpbox?ref=badge_large)