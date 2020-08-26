+++
title = "2018 - Ewasm 1.0"
date = 2018-01-01
+++

The team started the implementation of Ewasm 1.0 as defined in the
[design](https://github.com/ewasm/design), which included:

---

**[Hera (C++)](https://github.com/ewasm/hera) and [Hera.rs
(Rust)](https://github.com/ewasm/hera.rs)**: The ewasm 1.0 virtual machine which
can be integrated in existing Ethereum client compatible with
[EVMC](https://github.com/ethereum/evmc). Hera has support to different
WebAssembly interpreters and compilers such as:

- [Wabt](https://github.com/webassembly/wabt)
- [Binaryen](https://github.com/webassembly/binaryen)
- [WAVM](https://github.com/WAVM/WAVM)

---

**[Ewasm
Tests](https://github.com/ewasm/tests/tree/wasm-tests/src/GeneralStateTestsFiller/stEWASMTests)**:
Created test cases using the existing Ethereum tests infrastructure, generating
and executing tests using an Ethereum client compatible with Ewasm.

---

**[Sentinel Contract](https://github.com/ewasm/sentinel-rs)**: Ewasm Contract
(Written in Rust), validates and inject metering to contracts at deploy time.

---

**[ewasm-rust-api](https://github.com/ewasm/ewasm-rust-api)**: Rust library
which defines an Ewasm API that allows accessing Ewasm functions from your
contracts written in Rust.

**[Block Explorer (Etherchain
Light](https://github.com/ewasm/etherchain-light)**: Adapted existing Open
Source Project [Etherchain Light](https://github.com/gobitfly/etherchain-light)
to help us visualize blocks in the Ewasm testnet.

---

**Ewasm Testnet**: All these projects allowed to run an Ethereum 1.0 Testnet
with Ewasm Support, this means you could create contracts in a language
targetting EVM (i.e. Solidity), or you could write contracts using a language
targetting WebAssembly (Rust, C, AssemblyScript, etc), and live in the same
testnet.\
\
This tesnet used to live in this same address
(<http://ewasm.ethereum.org>), but currently is not being maintained. However
you can play with a Ewasm 1.0 Testnet in your local environment using this
repository: <https://github.com/jwasinger/ewasm-dev-env>.
