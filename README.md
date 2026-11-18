# EmbassyStarter

EmbassyStarter is a small `cargo-generate` template for experimenting with Embassy, the async embedded framework for Rust. It provides a starting project and dependency setup for STM32-based firmware.

The generated `main.rs` is intentionally just a `Hello, world!` placeholder. You will need to adapt the template to your board, add the appropriate target and memory configuration, and replace the example with your firmware. The current dependency setup is STM32-specific; the other family choices in the template are not ready to generate working projects.

## Generate a project

Install [`cargo-generate`](https://github.com/cargo-generate/cargo-generate), then run:

```sh
cargo generate --git https://github.com/BenMcAvoy/EmbassyStarter
```

Follow the prompts for the project name, author, license and STM32 board family. Review the generated manifest and configure the target for your specific board before building or flashing.

## About Embassy

Embassy provides async executors and embedded libraries for Rust microcontrollers. This template is an experiment and a starting point, not a maintained board support package. See the [Embassy documentation](https://embassy.dev/) for framework guidance.

The template includes Embassy's MIT license notice; keep the required attribution when reusing the scaffold.
