# aqua
Open source video (codec) hardware using riscv vector. (wish to be graphic also)

lowrisc ibex + vector (zve32x, 128 vlen)

# plan
1. QEMU to verify logic
2. 

# fpga

# build

## gnu toolchain(gcc + newlibc)
problem about thread not support
```
../configure --prefix=/opt/riscv --with-arch=rv32imc_zve32x --with-abi=ilp32
make newlib
```

## qemu ibex+vector
```
../configure --target-list=riscv32-softmmu,riscv32-linux-user --enable-debug --enable-linux-user --enable-kvm
ninja
```
