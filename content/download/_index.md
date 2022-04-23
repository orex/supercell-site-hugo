---
title: "Download and install"
date: 2018-12-29T11:02:05+06:00
icon: "fas fa-download"
type: "docs"
weight: 3
card:
  order: 2
  description: "Using supercell as easy as one-two-three. Check the to learn different methods of obtaining and using the program."
  btncaption: "Download"
  btnicon: "fas fa-download"
  highlighted: true
---

### Compiled binaries

The easiest way to obtain the program is to download compiled binaries for Linux, Mac and Windows platforms. Just download the archive, unpack it and follow the instruction inside. You don't need to install the binaries, therefore you can use it without a root permission. Previous major version (unsupported) of *supercell* v1.2 is available [here](https://github.com/orex/supercell/tree/gh-pages/v1.2)

{{< image-link link="external/exe/supercell-linux.tar.gz" img="/images/Linux64x64.png" caption="Linux 64bit" >}}
{{< image-link link="external/exe/supercell-osx.tar.gz" img="/images/mac64x64.png" caption="OSX" >}}
{{< image-link link="external/exe/supercell-windows.zip" img="/images/Windows64x64.png" caption="Windows x64" >}}

### Source code

You can also compile the program from [source code](https://github.com/orex/supercell/). To do so, you should have a knowledge of *git* and *cmake*. Please check file [.travis.yml](https://github.com/orex/supercell/blob/master/.travis.yml) for relevant commands. Compiling under Linux, OSX and FreeBSD should be relatively easy, but compiling on Windows you should be done from scratch.

### Other sources

Old version of the program is available in ArchLinux [repository](https://aur.archlinux.org/packages/supercell-git). I have a plan to make the program available via [snap](https://snapcraft.io).