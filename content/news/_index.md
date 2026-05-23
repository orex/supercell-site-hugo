---
title: "News"
date: 2022-04-12T11:11:11+06:00
draft: false
icon: "far fa-newspaper"
type: "docs"
card: false
weight: 10
---

#### 24-05-2026
**Supercell v2.1.2 (maintenance release)** Mostly a maintenance update: dependencies and packages were refreshed, several minor bugs were fixed, and benchmarks/tests show performance improved by almost 30%. New native builds are now published for **Linux ARM64 (Ubuntu)** and for **macOS Intel and Apple Silicon** separately. The x86_64 Linux binary from the site targets AVX-capable CPUs (any x86_64 from 2011 onward) and is built to run on Ubuntu 18.04+, Debian 10+, RHEL 8+ and openSUSE Leap 15.x+. Download [here](download).
#### 03-08-2024
**Supercell v2.1.1 (minor improvement)** External dependencies updated, minor bugs fixed. Download program [here](download).
<!--more-->
#### 03-11-2022
**Supercell v2.1.0** A new version of supercell program released with improvement of electrostatic calculation precision and performance. New multi-threading approach allows effectively parallelize program up to 64 threads. Please check [benchmark](benchmark) for relevant information.
#### 10-05-2022
**New supercell site and packages** Welcome to the new supercell site: a lot of useful information has been added. The program itself is now available via [snap](https://snapcraft.io/) and for the Linux ARM environment. See [download](download).
#### 02-01-2022
**Supercell v2.0.2 (minor bugfix)** Symmetry search in very sheared cells is improved. Gemmi and xxHash updated.
#### 20-05-2021
**Supercell v2.0** A new version of supercell program with major improvements: performance, portability and new parameters. Please check [changelog](version-2x) and [benchmark](benchmark).
#### 23-05-2019
**Supercell v1.2 (performance increase)** The new version of supercell program is around 4 times faster, than the previous one!
#### 09-02-2019
**Microsoft Windows support (experimental)** I would like to announce Microsoft Windows platform support. You can download the binary below. An output structures packing is not supported (`-a` option). The binary is tested on Windows 7 and Windows 10.
#### 24-01-2019
**Supercell v1.1** The maximum limit for processing structures has been increased. The new version of supercell program can process up to 10<sup>15</sup> total structures. This value is far beyond a reasonable limit due to calculation time. The average program performance is about 10-100 billion structures per day with a standard desktop processor. Feedback is very welcome.
