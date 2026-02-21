# Red Teamer Hacking

## Motivation
Upon learning much about Virtual Machines, CPU archs, binary dissections, etc., trying vulnerability research might be another way to learn new things when it comes to computing.

## Device
### Latitude 5300
uses vm kali-linux

## my roadmap
- learn basics on cpu flaws and common os protections
- try binary exploitation by writing and explicitly compiling vulnerable programs

## what i learned right now
- extensive use of gdb, and other improvements to gdb like `pwndbg` where it has `cyclic` to do fuzzing
- better to identify what your emulated machine config first before anything else.
- ASLR or Address Space Layout Randomization, randomizes memory everytime our program runs. disabling it helps predict the functions like `exit` fixed on memory layout, avoiding `segfaults`.
- directly writing raw bytes is always needs to be remember. On `python3` im using `print` function which treats our input as `unicode` chars, instead of raw byte. I fail on these, took too much time before i get my first `ret2func` exploit after resolving these. im [following these tutorial](https://www.ired.team/offensive-security/code-injection-process-injection/binary-exploitation/rop-chaining-return-oriented-programming) and it uses python2.

## Resources
- [ROP Chaining: Return Oriented Programming | Red Team Notes](https://www.ired.team/offensive-security/code-injection-process-injection/binary-exploitation/rop-chaining-return-oriented-programming)
