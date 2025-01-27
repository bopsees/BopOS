# The RIF OS

## Robot is Fat.

To start, load the kernel.iso from /dist/x86_64 into an emulator e.g QEMU

## Build instructions: (docker required)
docker run --rm -it -v "$(pwd)":/root/env myos-buildenv
make build-x86_64
exit docker
qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso