---
label: Configuration
order: 100
icon: file
---
# Node configuration

In this page, we will explain the relevant configuration information of the node. martiscoin is a platform built on Blockcore for building a first-layer consensus network based on the Bitcoin protocol. Therefore, the relevant configuration parameters remain consistent with Bitcoin.The node directory is as follows:

## Node Directory Path

!!!
The configuration file is in the node directory,[!badge msc.conf].
!!!

#### Windows

Enter the following command in the folder directory address bar.

```
%Appdata%\marscore
```

#### Linux

If you start the martiscoin node using the root account.

```
cd /root/.marscore
```

## Seed Nodes

These are seed nodes hosted by us. The network does not requires them to be up at all time because martiscoin is a decentralized network. However we provide them for others who can't run one for whatever reasons.

Location   | Endpoint
:---   |
Singapore | 
United State | 
Germany | 
Hong Kong | 

More additional node information can be found [here](https://explorer.martiscoin.org/network)

#### Add a node in the wallet interface

![Add Node](/static/config-1.png)

#### Add nodes using configuration files

!!!
xxx.xx.xx.xx is the IP address of other nodes.
!!!

Open the node file [!badge msc.conf] using Notepad, enter the following content and save. The configuration information takes effect after the node is restarted.

```
addnode=xxx.xx.xx.xx
addnode=xxx.xx.xx.xx
```


## RPC Settings

The RPC service supports most Bitcoin methods,[!badge server=1] Activate RPC Server (default: 0);Where the RPC Server binds (default: 127.0.0.1 and ::1);#Ip address allowed to connect to RPC (default all: 0.0.0.0 and ::)

```
server=1
rpcbind=127.0.0.1
rpcallowip=127.0.0.1
rpcuser=
rpcpassword=
```