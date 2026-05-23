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

* **Performance boost:** Almost half of the code was changed in this release to achieve a performance improvement. Algorithms for symmetry search, electrostatic calculation, file I/O and, of course, structure enumeration became 4-10 times faster than previously.
* **Multi-threading:** The enumeration algorithm can run in parallel on shared-memory architectures. No extra programs (like MPI) are needed. In this release, you can benefit from parallelization on up to 16 cores. The limit will be overcome in the next release.
* **Additional scenarios:** Supercell program can now be used to search for high-symmetry disorder supercells (`-n w` option). Randomness of output structures can be controlled by the random-seed option.
* **New I/O module:** Supercell program no longer uses the [OpenBabel](https://github.com/openbabel) library for I/O and structure processing. Reading and writing of CIF files is now done internally (thanks to the [gemmi](https://github.com/project-gemmi/gemmi) library for CIF parsing and spacegroup information). This approach improves performance and handles ambiguous spacegroup information and inconsistencies in CIF files much better.
* **New C++ standard:** Supercell code was updated to the C++14 standard. Support for old compilers has been dropped.
* **Dependency update:** Supercell v1.x code binaries (from the site) could be run successfully on Linux distributions from 2008 onward and supported all x86_64 processors newer than 2005. The new version is compiled with relatively recent compilers and does not support obsolete Linux. It supports, for example: Ubuntu 14.04 and newer; Debian 8 and newer; CentOS 7 and newer, etc. The CPU should be SSE2 compatible.
* **Windows version improvement:** Performance of the Windows version is significantly improved by using modern build toolchains. Archive output (`-a`) is also supported now.

Old version (v1.2) binaries are available [here](https://github.com/orex/supercell/tree/gh-pages/v1.2). Note that this version is no longer supported.
