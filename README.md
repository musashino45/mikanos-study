# mikanos
For about MikanOS studying.
dev env OS: Ubuntu22.04
target CPU: AMD64

# reference

https://github.com/uchan-nos/mikanos

http://zero.osdev.jp/

# build method
1. kernel build "compiling and linking"
```bash
$ cd ~/workspace/mikanos/kernel
$ make //for detail, please refer to Makefile
```

2. bootloader build
```bash
$ cd ~/edk2
$ source edksetup.sh //if build doesn't work well
$ build
$ ~/osbook/devenv/run_qemu.sh Build/MikanLoaderX64/DEBUG_CLANG38/X64/Loader.efi ~/workspace/mikanos/kernel/kernel.elf
```

Regular maintenance is scheduled :)
