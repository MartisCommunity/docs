---
icon: note
---
# Run Martiscoin node


Martiscoin node integrates wallet and miner.For operations on martiscoin, you need a node instance running on your computer. Currently, precompiled node executables are available for Windows, Linux. Once started, the node will start synchronizing the blockchain, and once completed, you can operate with the wallet and start mining.

## Windows

#### Install .Net SDK 8.0.404

First install the Microsoft .NET8 base library. The link below contains the installation address of the library. You can choose the corresponding version to install according to the system version. By default, it is recommended to install the .NET8 SDK complete installation package.

```
https://dotnet.microsoft.com/en-us/download/dotnet/thank-you/sdk-8.0.404-windows-x64-installer
```

#### Download node and run

Double click the [!badge Martiscoin.Node.exe] to start Martiscoin node.After the startup is complete, the wallet can be created through a web browser.
![Run a Martiscoin node](/static/node-1.png)


## Linux(Ubuntu 24.10)

!!!
For more information about .NET8 installation you can check [here](
https://learn.microsoft.com/en-us/dotnet/core/install/linux-ubuntu-install?tabs=dotnet8&pivots=os-linux-ubuntu-2410).
!!!

#### Install the SDK

The .NET SDK allows you to develop apps with .NET. If you install the .NET SDK, you don't need to install the corresponding runtime. To install the .NET SDK, run the following commands:

```
sudo apt-get update && \
sudo apt-get install -y dotnet-sdk-8.0
```

#### Download node and run

Download the node file and after decompression is complete, enter the following command

```
dotnet Martiscoin.Node.dll
```
If you see the following screenshot interface, it means that the node has been running successfully.

![Run a Martiscoin node](/static/node-2.png)