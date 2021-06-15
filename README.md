# MCCI Catena 4610 Board Support Crate

## About

This is an unofficial Board Support Crate (BSC) for using the [MCCI Catena 4610] Integrated Node for LoRaWAN technology with the [Rust] programming language.

It is currently in its early stages. Documentation is sparse and features are basic. Pull requests welcome!

[MCCI Catena 4610]: https://store.mcci.com/collections/lorawan-iot-and-the-things-network/products/mcci-catena-4610-integrated-node-for-lorawan-technology
[Rust]: https://www.rust-lang.org/


## Usage

Currently, two ways for flashing code to the Gnat are supported:
- Using the built-in bootloader via [dfu-util].
- Using an external STLINK programmer via [cargo-embed].

To flash an example using `dfu-util`, run something like this:

```
cargo run --example led
```

To flash an example using `cargo-embed`, run something like this:

```
cargo embed --example led
```

[dfu-util]: http://dfu-util.sourceforge.net/
[cargo-embed]: https://github.com/probe-rs/cargo-embed


## License

This project is open source software, licensed under the terms of the [Zero Clause BSD License][] (0BSD, for short). This basically means you can do anything with the software, without any restrictions, but you can't hold the authors liable for problems.

See [LICENSE.md] for full details.

[Zero Clause BSD License]: https://opensource.org/licenses/0BSD
[LICENSE.md]: https://github.com/braun-embedded/rust-catena-4610/blob/master/LICENSE.md
