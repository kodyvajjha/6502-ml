# 6502-ml
6502 chip family simulator in OCaml

Exposed as a library through `cpu.mli`  
`jbuilder build unit_test.exe` creates `_build/default/unit_test.exe` which takes a path to a ROM in argument and launch the CPU on it, beginning at `PC=0x400`, stopping when encountering a trap.  

The CPU passes all functional tests of [Klaus Dormann's test suite](https://github.com/Klaus2m5/6502_65C02_functional_tests) (`test.bin` is an assembled of `6502_functional_test.a65)  

It's zero page starts at address `0x0000`
