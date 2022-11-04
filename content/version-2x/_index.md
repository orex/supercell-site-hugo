---
title: "Whats new 2.x"
date: 2022-04-12T11:11:11+06:00
type: "docs"
weight: 20
card:
  order: 1
  description: "Supercell 2.x is a major supercell release with significant performance boost, multithreading support and code improvement and refactoring."
  btncaption: "Read more"
  btnicon: "far fa-arrow-alt-circle-up"
  highlighted: false
---

I'm proud to present you a new version of supercell program. This is a major release with several significant changes:

* **Performance boost:** Almost half of the code was changed in the release to achieve performance improvement. Algorithms for symmetry search, electrostatic calculation, file I/O and, of course, structures enumeration became 4-10 times faster then previously.
* **Multi threading:** Enumeration algorithm can run in parallel on shared memory architectures. No extra programs (like MPI) are needed. In this release, you can gain from parallelization on up to 16 cores. The limit will be overcome with the next release.
* **Additional scenarios:** Supercell program can be used now for searching of high symmetry disorder supercell (`-n w` option). Randomness of output structures can be controlled by random-seed option.
* **New I/O module:** Supercell program doesn't use [OpenBabel](https://github.com/openbabel) library for I/O and structures processing anymore. Reading and writing of CIF files now is done internally (thanks to [gemmi](https://github.com/project-gemmi/gemmi) library for cif parsing and spacegroup information). Such approach allows to increase performance and treat ambiguous spacegroup information and inconsistency in CIF files much better.
* **New C++ standard:** Supercell code was updated to C++14 standard. Support for old compilers has been dropped.
* **Dependency update:** Supercell v1.x code binaries (from the site) can be run successfully on Linux distribution from 2008 year up to now and support all x86_64 processors younger than year 2005. New version is compiled with relatively recent compilers and does not support obsolete Linux. It supports for example: Ubuntu 14.04 and newer; Debian 8 and newer; CentOS 7 and newer etc. The CPU should be SSE2 compatible.
* **Windows version improvement:** Performance of Windows version is significantly improved by using modern build chains. Archive output (`-a`) is also supported now.

Old version (v1.2) binaries  are available [here](https://github.com/orex/supercell/tree/gh-pages/v1.2). Note that this version is no longer supported.
