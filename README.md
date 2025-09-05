# RISC-V Bare Metal Rust example (with dynamic memory allocation)

This example must be built with nightly `cargo`, and the target
`riscv64imac-unknown-none-elf` must be installed to the nightly.

1. `rustup toolchain install nightly`
2. `rustup target add riscv64imac-unknown-none-elf`

Build with:

```
cargo build
```

Run on QEMU:

```
qemu-system-riscv64 -machine virt -bios target/riscv64imac-unknown-none-elf/debug/risc-v-rust-bare-metal -nographic
```

Sample output:

```
Hello, world!
A string
```

## Article

This code is meant to accompany the article at
http://popovicu.com/posts/bare-metal-rust-risc-v-with-dynamic-memory
