---
title: "Download and install"
date: 2022-04-12T11:11:11+06:00
icon: "fas fa-download"
type: "docs"
weight: 30
card:
  order: 2
  description: "Using supercell is as easy as one-two-three. Check this page to learn different methods of obtaining and using the program."
  btncaption: "Download"
  btnicon: "fas fa-download"
  highlighted: true
---

### Compiled binaries

The easiest way to obtain the program is to download compiled binaries for Linux, Mac and Windows platforms. Just download the archive, unpack it and follow the instruction inside. You don't need to install the binaries, therefore you can use it without a root permission. The latest binaries (currently **v2.1.2**) are published on [GitHub Releases](https://github.com/orex/supercell/releases/latest). The previous versions (unsupported) of *supercell* are available in [archive](download/archive).

{{< image-link link="https://github.com/orex/supercell/releases/download/v2.1.2/supercell-linux.tar.gz" img="images/Linux64x64.png" caption="Linux x86_64" >}}
{{< image-link link="https://github.com/orex/supercell/releases/download/v2.1.2/supercell-linux-arm64.tar.gz" img="images/Linux64x64-ARM.png" caption="Linux ARM64 (Ubuntu)" >}}
{{< image-link link="https://github.com/orex/supercell/releases/download/v2.1.2/supercell-osx-intel.tar.gz" img="images/mac64x64.png" caption="macOS Intel" >}}
{{< image-link link="https://github.com/orex/supercell/releases/download/v2.1.2/supercell-osx.tar.gz" img="images/mac64x64-ARM.png" caption="macOS Apple Silicon" >}}
{{< image-link link="https://github.com/orex/supercell/releases/download/v2.1.2/supercell-windows.zip" img="images/Windows64x64.png" caption="Windows x64" >}}

The x86_64 Linux binary targets AVX-capable CPUs (any x86_64 from 2011 onward) and links against glibc no newer than 2.28, so it runs on Ubuntu 18.04+, Debian 10+, RHEL 8+, openSUSE Leap 15.x+ and other distributions of similar vintage. Linux ARM64 binaries are now available directly (no longer beta-only via snap).

### Snap store (Linux)

Another modern option is to install the program via snap. Available both for Intel/AMD and ARM (experimental) architectures.

<a href="https://snapcraft.io/supercell">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/static/images/badges/en/snap-store-white.svg" />
  <p></p>
</a>

This is available for almost all modern Linux distributions and is as easy as clicking the link above (Web UI) or running the command in a terminal:

```
sudo snap install supercell
```

Be careful, *snap* is a very secure way of installing programs. Therefore, you can get a permission error in case of running the program outside your home folder.

### Repository (ArchLinux)

Old version of the program (v1.2) is available in ArchLinux [repository](https://aur.archlinux.org/packages/supercell-git).

### Source code

You can also compile the program from [source code](https://github.com/orex/supercell/). To do so, you should have knowledge of *git* and *cmake*. Please check github actions file [supercell-cicd.yml](https://github.com/orex/supercell/blob/master/.github/workflows/supercell-cicd.yml) for relevant commands. Please use latest version of OneAPI-tbb for the best performance. Compiling under Linux, OSX and FreeBSD should be relatively easy, but compiling on Windows should be done from scratch.
