# SH-DOS
 An x86_64 Operating System written in Assembly, inspired by MS-DOS and UNIX commands.

---

# Current Version

The current version is PRE-ALPHA 0x00. This version it's just for some tests with 16 bits Assembly, like write `Welcome to SH-DOS!` on the screen. In the next release, I will begin the development of a transition from REAL mode to PROTECTED mode.

# TODO list

- [x] Show "WELCOME TO SH-DOS!" on the screen
- [ ] Transition (REAL MODE to PROTECTED MODE)
- [ ] Show "PROTECTED MODE" on the screen

#  About the project

This isn't a professional Operating System, it's just a little project for me to learn how an Operating System works, how it processes data, and how it can run commands. I'm not an tech expert, I'm just a teen who wants to discover the underworld of the computers.

# How to run

These commands are focused on `Debian GNU/Linux 13` users. You need some packages installed, like `nasm` and `qemu-system`. To install, run:

```bash
$ sudo apt update
$ sudo apt upgrade -y
$ sudo apt install nasm qemu-system -y
```

And to run the `boot.asm` file, run:

```bash
$ nasm -f bin boot.asm -o boot.bin    # compiles the boot program
$ qemu-system-x86_64 -drive format=raw,file=boot.bin    # run the file on a VM
```
