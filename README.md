# [pimoroni-interstate75] - Board Support for the [Pimoroni Interstate 75]

You should include this crate if you are writing code that you want to run on
a [Pimoroni Interstate 75] - an LED matrix driver board based on the RP2040.

This crate includes the [rp2040-hal], but also configures each pin of the
RP2040 chip according to how it is connected up on the Interstate 75.

[Pimoroni Interstate 75]: https://shop.pimoroni.com/products/interstate-75
[pimoroni-interstate75]: https://github.com/rp-rs/rp-hal-boards/tree/main/boards/pimoroni_interstate75
[rp2040-hal]: https://github.com/rp-rs/rp-hal/tree/main/rp2040-hal
[Raspberry Silicon RP2040]: https://www.raspberrypi.org/products/rp2040/

## Examples

Examples in this repository are set up assuming you have [elf2uf2-rs] installed.
A `.cargo/config.toml` file is included.

### Blinky

This example will flash the LEDs on the I75 board, in a red-green-blue pattern.
It does not require anything to be connected to the HUB75 connector.

```plaintext
$ cargo run --release --example blinky.rs
```

[elf2uf2-rs]: https://github.com/JoNil/elf2uf2-rs
