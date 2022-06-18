# license

[![Rust](https://github.com/evenorog/license/actions/workflows/rust.yml/badge.svg)](https://github.com/evenorog/license/actions/workflows/rust.yml)
[![Crates.io](https://img.shields.io/crates/v/license.svg)](https://crates.io/crates/license)
[![Docs](https://docs.rs/license/badge.svg)](https://docs.rs/license)

Provides embedded license information from [SPDX](https://spdx.org).

```rust
let apache2 = "Apache-2.0".parse::<&dyn License>().unwrap();
assert_eq!(apache2.name(), "Apache License 2.0");
```

License exceptions are also supported.

```rust
let gcc = "GCC-exception-3.1".parse::<&dyn Exception>().unwrap();
assert_eq!(gcc.name(), "GCC Runtime Library exception 3.1");
```

### License

Licensed under either of

 * Apache License, Version 2.0, ([LICENSE-APACHE](LICENSE-APACHE) or http://www.apache.org/licenses/LICENSE-2.0)
 * MIT license ([LICENSE-MIT](LICENSE-MIT) or http://opensource.org/licenses/MIT)

at your option.

### Contribution

Unless you explicitly state otherwise, any contribution intentionally submitted
for inclusion in the work by you, as defined in the Apache-2.0 license, shall be dual licensed as above, without any
additional terms or conditions.
