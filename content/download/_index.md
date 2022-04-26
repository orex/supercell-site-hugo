---
title: "Download and install"
date: 2022-04-12T11:11:11+06:00
icon: "fas fa-download"
type: "docs"
weight: 30
card:
  order: 2
  description: "Using supercell is as easy as one-two-three. Check the to learn different methods of obtaining and using the program."
  btncaption: "Download"
  btnicon: "fas fa-download"
  highlighted: true
---

### Compiled binaries

The easiest way to obtain the program is to download compiled binaries for Linux, Mac and Windows platforms. Just download the archive, unpack it and follow the instruction inside. You don't need to install the binaries, therefore you can use it without a root permission. The previous major version (currently unsupported) of *supercell* v1.2 is available [here](https://github.com/orex/supercell/tree/gh-pages/v1.2)

{{< image-link link="external/exe/supercell-linux.tar.gz" img="/images/Linux64x64.png" caption="Linux x86_64" >}}
{{< image-link link="external/exe/supercell-osx.tar.gz" img="/images/mac64x64.png" caption="OSX Intel" >}}
{{< image-link link="external/exe/supercell-windows.zip" img="/images/Windows64x64.png" caption="Windows x64" >}}
{{< image-link link="external/exe/supercell-linux-arm64.tar.gz" img="/images/Linux64x64-ARM.png" caption="Linux ARM64" >}}

Please note that the last link is to Linux ARM64 architecture. The support is in **beta** stage.

### Snap store (Linux)

Another very modern option is to install program via snap. Availabe both for Intel/AMD and ARM (experimental) architectures.

<a href="https://snapcraft.io/supercell">
  <img alt="Get it from the Snap Store" src="https://snapcraft.io/static/images/badges/en/snap-store-white.svg" />
  <p></p>
</a>

This is available for almost all modern Linux distribution and is as easy as to click on the link above (Web UI) or to write the command in terminal:

```
sudo snap install supercell
```

### Repository (ArchLinux)

Old version of the program is available in ArchLinux [repository](https://aur.archlinux.org/packages/supercell-git).

### Source code

You can also compile the program from [source code](https://github.com/orex/supercell/). To do so, you should have knowledge of *git* and *cmake*. Please check file [.travis.yml](https://github.com/orex/supercell/blob/master/.travis.yml) for relevant commands. Compiling under Linux, OSX and FreeBSD should be relatively easy, but compiling on Windows should be done from scratch.
