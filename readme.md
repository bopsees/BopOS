# The RIF OS

## Robot is Fat.

To start, load the kernel.iso from /dist/x86_64 into an emulator e.g QEMU

## Build instructions: (docker required)
docker run --rm -it -v "$(pwd)":/root/env myos-buildenv <br>
make build-x86_64 <br>
exit docker <br>
qemu-system-x86_64 -cdrom dist/x86_64/kernel.iso <br>