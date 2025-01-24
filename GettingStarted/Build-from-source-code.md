---
order: 100
icon: git-compare
---
# Build from Source code

This guide will help you build the Marscoin software from the source code.

The software is divided into two parts:

Wallet: the graphical interface that allows you to manage your accounts and transactions.

Miner: the part of the software that allows you to mine new blocks and earn rewards.

Building the software from the source code is useful for developers, testers, and users who want to have the latest version of the software or want to contribute to the project. It is also the most secure way to get the software as you can verify the source code before building it and remove the need to trust pre-built binaries.

This guide assumes that you have a basic understanding of the Visual Studio and that you have the necessary tools installed on your device.

---

## Supported Platforms

- Windows - works from Windows 7 and later, on both x86 and x64 architecture. Most of the development and testing is happening here.

- Linux - works and Ubuntu 14.04 and later (x64). It's been known to run on some other distros so your mileage may vary.

- MacOS - works from OSX 10.12 and later.

## Prerequisites

To compile and run the node, you need

- [!badge .NET8]
- [!badge Visual Studio 2022]

---

## How to build from sources


#### Cloning the Repo

Now that we have git we can clone the Warthog repository from GitHub:

```
git clone https://github.com/martiscoin/node.git
```

#### Compiling

Open the [!badge Martiscoin.sln] file using [!badge Visual Studio 2022], set [!badge Martiscoin.Node] as the startup project, and click run.