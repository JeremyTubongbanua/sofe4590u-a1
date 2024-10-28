## x86

```bash
sudo apt install -y qemu-system-x86 gcc
gcc -o hello_x86 hello.c
qemu-x86_64 -L /usr/lib ./hello_x86
```

## ARM (aarch64)

```bash
sudo apt install -y qemu-system-aarch64 gcc-aarch64-linux-gnu
aarch64-linux-gnu-gcc -o hello_aarch64 hello.c
qemu-aarch64 -L /usr/aarch64-linux-gnu ./hello_aarch64 
```

## MIPS

```bash
sudo apt install -y qemu-system-mips gcc-mips-linux-gnu
mips-linux-gnu-gcc -o hello_mips hello.c
qemu-mips -L /usr/mips-linux-gnu ./hello_mips 
```

## RISC-V (riscv64)

```bash
sudo apt install -y qemu-system-misc gcc-riscv64-linux-gnu
riscv64-linux-gnu-gcc -o hello_riscv64 hello.c
qemu-riscv64 -L /usr/riscv64-linux-gnu ./hello_riscv64
```
