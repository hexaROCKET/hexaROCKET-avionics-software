# hexaROCKET Avionics Software



This repository provides the library, build system, and test suite for the
hexaROCKET Avionics system. To meet the 
[goal](https://hexarocket.github.io/hexaROCKET-website/docs/project_overview/goals/) 
of the hexaROCKET project, a number of 
[sensors](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/sensors/)
are required. To iterate and achieve the mission, this data must also be 
[stored](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/flight-data/) 
and [transmitted](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/telemetry/) 
to the ground station. All of these tasks are the responsibility of the 
[avionics](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/overview/) system.

<br>

## Documentation

**[General Documentation](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/overview/)**

**[Rust Generated Docs]()**

## Getting Started

**You can also use the** 
**[Setup Guide](https://hexarocket.github.io/hexaROCKET-website/docs/avionics/setup/) to get started.**

### Prerequisites

1. Install the [Rust](https://www.rust-lang.org/tools/install) programming language

2. Clone this repository

3. Ensure you have the most up to date version of Rust:

```bash
rustup self update
rustup update stable
```

4. Add the ARM Cortex-M build target to Rust:

```bash
rustup target add thumbv6m-none-eabi
```

5. Add the uf2 imaging tool and SWD probe-run crate:

```
# Useful to creating UF2 images for the RP2040 USB Bootloader
cargo install elf2uf2-rs --locked
# Useful for flashing over the SWD pins using a supported JTAG probe
cargo install probe-run
```

## License

