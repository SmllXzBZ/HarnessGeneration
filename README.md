# HarnessGen
Some methods for generating harness/driver of library automatically.

## Paper

1. A Case Study on Automated Fuzz Target Generation for Large Codebases.[ESEM 2019](https://ieeexplore.ieee.org/document/8870150)
2. APICRAFT: Fuzz Driver Generation for Closed-source SDK Libraries.[Usenix 2021](https://www.usenix.org/system/files/sec21-zhang-cen.pdf)
3. DeepFuzz: Automatic Generation of Syntax Valid C Programs for Fuzz Testing.[AAAI 2019](https://faculty.ist.psu.edu/wu/papers/DeepFuzz.pdf)
4. FUDGE: fuzz driver generation at scale.[ESEC/FSE 2019](https://dl.acm.org/doi/pdf/10.1145/3338906.3340456)
5. FuzzBuilder: automated building greybox fuzzing environment for C/C++ library.[ACSAC 2019](https://dl.acm.org/doi/pdf/10.1145/3359789.3359846)
6. FuzzGen: Automatic Fuzzer Generation.[Usenix 2020](https://www.usenix.org/system/files/sec20fall_ispoglou_prepub.pdf)
7. IntelliGen: Automatic Driver Synthesis for Fuzz Testing.[ICSE-SEIP 2021](http://www.wingtecher.com/themes/WingTecherResearch/assets/papers/icse_seip_0221.pdf)
8. RULF: Rust Library Fuzzing via API Dependency Graph Traversal.[ASE 2021](https://arxiv.org/pdf/2104.12064.pdf)
9. SyRust: automatic testing of Rust libraries with semantic-aware program synthesis.[PLDI 2021](https://sat-group.github.io/ruben/media/pldi21-syrust.pdf)
10. WINNIE : Fuzzing Windows Applications with Harness Synthesis and Fast Cloning.[NDSS 2021](https://taesoo.kim/pubs/2021/jung:winnie.pdf)

## Open-source Tools

1. [gofuzzgen](https://github.com/kimuson13/gofuzzgen)

> gofuzzgen is generate template of fuzzing test code. 
> `Go`, `Golang`

2. [WINNIE](https://github.com/sslab-gatech/winnie)

> The forkserver calls the target's functionality under test through a harness. The harness is a dll specified in the AFL command-line and will get loaded by the fork-server. This harness is essentially responsible for acting as a shim between the forkserver and the target program. 
> `C`, `C++`

3. [Caffeine-harness](https://github.com/insufficiently-caffeinated/fuzzing-harnesses)

> This repo contains a set of fuzzing harnesses for use with caffeine. It also has cmake configuration that makes compiling such a fuzzing harness easy.
> `C`

4. [APICraft](https://github.com/occia/apicraft)

> This prototype is presented in USENIX 2021 as "APICraft: Fuzz Driver Generation for Closed-source SDK Libraries".
> `Objective-C++`

5. [autoharness](https://github.com/parikhakshat/autoharness)

> AutoHarness is a tool that automatically generates fuzzing harnesses for you. This idea stems from a concurrent problem in fuzzing codebases today: large codebases have thousands of functions and pieces of code that can be embedded fairly deep into the library. It is very hard or sometimes even impossible for smart fuzzers to reach that codepath. Even for large fuzzing projects such as oss-fuzz, there are still parts of the codebase that are not covered in fuzzing. Hence, this program tries to alleviate this problem in some capacity as well as provide a tool that security researchers can use to initially test a code base. This program only supports code bases which are coded in C and C++.
> `C`, `CodeQL`

6. [binja-fuzzit](https://github.com/bsw4p/binja-fuzzit)

> Generate a fuzzing harness for (shared) libraries from Binary Ninja.
> `Python`

7. [FuzzGen](https://github.com/HexHive/FuzzGen)

> FuzzGen, is a tool for automatically synthesizing fuzzers for complex libraries in a given environment. FuzzGen leverages a whole system analysis to infer the library’s interface and synthesizes fuzzers specifically for that library.
> FuzzGen is fully automatic and can be applied to a wide range of libraries. The generated fuzzers leverage LibFuzzer to achieve better code coverage and expose bugs that reside deep in the library.
> `C`, `C++`

8. [auto-fuzz-test](https://github.com/rust-fuzz/auto-fuzz-test)

> Fuzzing is a great (pen)testing tool, as long as you have one or just a handful of functions you want to fuzz. Fuzzing libpng is no problem, but fuzzing something like OpenSSL is nigh-impossible because you need to manually write the fuzzing boilerplate for every single function.
> This is an attempt to make fuzzing libraries with large API surfaces feasible by auto-generating the boilerplate. 
> `Rust`

9. [FuzzBuilder](https://github.com/hksecurity/FuzzBuilder)

> FuzzBuilder is a tool for generating an executable automatically for library fuzzing by using a unit test. Further, FuzzBuilder can generate seed files to fuzz a specific library API function by analyzing a unit test. 
> `C`, `C++`

10. [FuzzBuilderEx](https://github.com/kppw99/FuzzBuilderEx)

> Above the FuzzBuilder.

11. [RULF](https://github.com/Artisan-Lab/RULF)

> This prototype tool is aimed at generating fuzz targets for Rust libraries automatically. A fuzz target is a function that accepts an array of bytes and exercises some library APIs. The targets generated by our tool is a set of shallow fuzz targets (the length of each target is mostly smaller than or equal to 3) to cover as many library APIs as possible. Each generated target can be compiled successfully. Then, you can fuzz these targets with afl.rs to find potential bugs.
> `Rust`

12. [DeepFuzz](https://github.com/BambooL/DeepFuzz-AAAI-19)

## Some tools about fuzzing libraries

1. [Sloth](https://github.com/ant4g0nist/Sloth)

> Sloth is a fuzzing setup that makes use of libFuzzer and QEMU’s user-mode emulation (qemu/linux-user) on x86_64/aarch64 host to emulate aarch64 Android libraries to fuzz the target Android native library.
> `C++`, `C`

2. [CryptoFuzz](https://github.com/guidovranken/cryptofuzz)

> Differential cryptography fuzzing

3. [DeepFuzzer](https://github.com/G0o9leA1/DeepFuzzer)

> Fuzz the inner functions in libraries.
> `Python`


