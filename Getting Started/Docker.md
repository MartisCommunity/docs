---
order: 90
icon: cloud
tags: [guide]
---
# Docker

Docker is a platform for developers and sysadmins to develop, deploy, and run applications with containers. It uses Linux containers to deploy applications to any machine and treat them as a single server.

In case you prefer to use Docker, we provide a Docker image for each part of Marscoin.


## Wallet

The wallet is used to manage your wallet on the network.

You can easily download the image from the Docker Hub.

```
docker pull marscoin/daemon
```


## CPU Miner

The miner performs Proof-Of-Work consensus computations on blocks to secure the network. It must be connected to a daemon to work properly.

You can easily download the image from the Docker Hub.

```
docker pull marscoin/cupminer
```

## GPU Miner

Update to the latest release of Retype using one of the following commands for the package manager that you initially installed Retype with. For instance, if you used `npm` to install Retype, run the `npm` update command to update Retype locally.

```
docker pull marscoin/gpuminer
```


---

## Uninstall

Done with Retype? It's okay, we understand. :cry:

Uninstalling Retype is just as simple as installing. Use the same package manager to uninstall as you did to install. For instance, if you used `npm` to install Retype, run the `npm` uninstall command to remove.

+++ npm
```
npm uninstall retypeapp --global
```
+++ yarn
```
yarn global remove retypeapp
```
+++ dotnet
```
dotnet tool uninstall retypeapp --global
```
+++

All Retype related files and folders within your project can be deleted, such as the **retype.yml** file and the generated `.retype` folder.

---

## Platform specific

The default `retypapp` **NPM** package is a bundle of several platform specific packages. The installer will automatically detect and choose the correct platform package from the bundle during installation.

The bundle provides convenience although at the cost of an increased download size.

The **dotnet** package installer will automatically download the platform specific package.

For **NPM** and **Yarn**, it is possible to install smaller platform specific packages without the bundling. Currently, four separate platforms are supported and can be installed independently from the primary `retypeapp` package.

### :icon-package: macOS

+++ npm
```
npm install retypeapp-darwin-x64 --global
```
+++ yarn
```
yarn global add retypeapp-darwin-x64
```
+++ dotnet
```
dotnet tool install retypeapp --global
```
+++

{.compact}
OS                                    | Version                 | Architectures     |
--------------------------------------|-------------------------|-------------------|
[macOS][macOS]                        | 10.15+                  | x64, Arm64        |

[macOS]: https://support.apple.com/macos

### :icon-package: Windows

+++ npm
```
npm install retypeapp-win-x64 --global
# or
npm install retypeapp-win-x86 --global
```
+++ yarn
```
yarn global add retypeapp-win-x64
# or
yarn global add retypeapp-win-x86
```
+++ dotnet
```
dotnet tool install retypeapp --global
```
+++

{.compact}
OS                                    | Version                 | Architectures     |
--------------------------------------|-------------------------|-------------------|
[Windows 10 Client][Windows-client]   | Version 1607+           | x64, x86, Arm64   |
[Windows 11][Windows-client]          | Version 22000+          | x64, x86, Arm64   |
[Windows Server][Windows-Server]      | 2012+                   | x64, x86          |
[Windows Server Core][Windows-Server] | 2012+                   | x64, x86          |
[Nano Server][Nano-Server]            | Version 1809+           | x64               |

[Windows-client]: https://www.microsoft.com/windows/
[Windows-lifecycle]: https://support.microsoft.com/help/13853/windows-lifecycle-fact-sheet
[win-client-docker]: https://hub.docker.com/_/microsoft-windows
[Windows-Server-lifecycle]: https://learn.microsoft.com/windows-server/get-started/windows-server-release-info
[Nano-Server]: https://learn.microsoft.com/windows-server/get-started/getting-started-with-nano-server
[Windows-Server]: https://learn.microsoft.com/windows-server/

### :icon-package: Linux

+++ npm
```
npm install retypeapp-linux-x64 --global
```
+++ yarn
```
yarn global add retypeapp-darwin-x64
```
+++ dotnet
```
dotnet tool install retypeapp --global
```
+++

{.compact}
OS                                    | Version               | Architectures     |
--------------------------------------|-----------------------|-------------------|
[Alpine Linux][Alpine]                | 3.15+                 | x64, Arm64, Arm32 |
[CentOS Linux][CentOS]                | 7                     | x64               |
[CentOS Stream Linux][CentOS]         | 8                     | x64               |
[Debian][Debian]                      | 10+                   | x64, Arm64, Arm32 |
[Fedora][Fedora]                      | 36+                   | x64               |
[openSUSE][OpenSUSE]                  | 15+                   | x64               |
[Oracle Linux][Oracle-Linux]          | 7+                    | x64               |
[Red Hat Enterprise Linux][RHEL]      | 7+                    | x64, Arm64        |
[SUSE Enterprise Linux (SLES)][SLES]  | 12 SP2+               | x64               |
[Ubuntu][Ubuntu]                      | 18.04+                | x64, Arm64, Arm32 |

[Alpine]: https://alpinelinux.org/
[Alpine-lifecycle]: https://alpinelinux.org/releases/
[CentOS]: https://www.centos.org/
[CentOS-lifecycle]:https://wiki.centos.org/FAQ/General
[CentOS-docker]: https://hub.docker.com/_/centos
[CentOS-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-centos8
[Debian]: https://www.debian.org/
[Debian-lifecycle]: https://wiki.debian.org/DebianReleases
[Debian-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-debian10
[Fedora]: https://getfedora.org/
[Fedora-lifecycle]: https://fedoraproject.org/wiki/End_of_life
[Fedora-docker]: https://hub.docker.com/_/fedora
[Fedora-msft-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-fedora32
[Fedora-pm]: https://fedoraproject.org/wiki/DotNet
[OpenSUSE]: https://opensuse.org/
[OpenSUSE-lifecycle]: https://en.opensuse.org/Lifetime
[OpenSUSE-docker]: https://hub.docker.com/r/opensuse/leap
[OpenSUSE-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-opensuse15
[Oracle-Linux]: https://www.oracle.com/linux/
[Oracle-Lifecycle]: https://www.oracle.com/a/ocom/docs/elsp-lifetime-069338.pdf
[RHEL]: https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux
[RHEL-lifecycle]: https://access.redhat.com/support/policy/updates/errata/
[RHEL-msft-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-rhel8
[RHEL-pm]: https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/8/html/developing_.net_applications_in_rhel_8/using-net-core-on-rhel_gsg#installing-net-core_gsg
[SLES]: https://www.suse.com/products/server/
[SLES-lifecycle]: https://www.suse.com/lifecycle/
[SLES-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-sles15
[Ubuntu]: https://ubuntu.com/
[Ubuntu-lifecycle]: https://wiki.ubuntu.com/Releases
[Ubuntu-pm]: https://learn.microsoft.com/dotnet/core/install/linux-package-manager-ubuntu-2004
[glibc]: https://www.gnu.org/software/libc/
[musl]: https://musl.libc.org/