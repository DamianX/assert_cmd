# assert_cmd

> **Assert `process::Command`** - Easy command initialization and assertions.

[![Build Status](https://dev.azure.com/assert-rs/assert-rs/_apis/build/status/assert_cmd?branchName=master)](https://dev.azure.com/assert-rs/assert-rs/_build/latest?definitionId=3&branchName=master)
[![Documentation](https://img.shields.io/badge/docs-master-blue.svg)][Documentation]
![License](https://img.shields.io/crates/l/assert_cmd.svg)
[![Crates Status](https://img.shields.io/crates/v/assert_cmd.svg)](https://crates.io/crates/assert_cmd)

## Install

Add to your `Cargo.toml`:

```toml
[dependencies]
assert_cmd = "0.11"
```

## Example

Here's a trivial example:

```rust,no_run
use assert_cmd::Command;

let mut cmd = Command::cargo_bin("bin_fixture").unwrap();
cmd.assert().success();
```

## Relevant crates

Other crates that might be useful in testing command line programs.
* [duct][duct] for orchestrating multiple processes.
* [rexpect][rexpect] for testing interactive programs.
* [`assert_fs`][assert_fs] for filesystem fixtures and assertions.
* [dir-diff][dir-diff] for testing file side-effects.
* [tempfile][tempfile] for scratchpad directories.

[rexpect]: https://crates.io/crates/rexpect
[dir-diff]: https://crates.io/crates/dir-diff
[tempfile]: https://crates.io/crates/tempfile
[duct]: https://crates.io/crates/duct
[assert_fs]: https://crates.io/crates/assert_fs

## License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally
submitted for inclusion in the work by you, as defined in the Apache-2.0
license, shall be dual licensed as above, without any additional terms or
conditions.

[Crates.io]: https://crates.io/crates/assert_cmd
[Documentation]: https://docs.rs/assert_cmd
