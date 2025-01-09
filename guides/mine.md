---
label: How to mine
icon: rocket
order: 30
---
# How to mine

!!!
This guide contains all needed information to start mining Martiscoin, on your own node.
!!!

Martiscoin is a Proof of Work (PoW) blockchain, which means that miners must solve complex mathematical problems to add new blocks to the blockchain and receive rewards. Their tasks are to find a hash that matches the difficulty target set by the network, ensuring that the block is valid and accepted by the network.

The main role of the miner is to secure the network by validating transactions and adding them to the blockchain.

Martiscoin node integrates wallet and miner.You only need to enable relevant configurations in the node configuration to automatically enter cycle mining.Before you can start mining, you must first create a wallet.

---

## Start Mining

Martiscoin supports CPU and GPU mining. 

>NOTE: A node can only run one mining method.

Open the node file [!badge msc.conf] using Notepad, enter the following content and save. The configuration information takes effect after the node is restarted.

### CPU

The mining address must belong to the current node wallet address;[!badge mine=1] Indicates enabling mining;[!badge minethreads=1] Indicates the number of CPU threads used for mining.

```
mineaddress=
mine=1
minethreads=1
```

### GPU

The mining address must belong to the current node wallet address;[!badge mine=1] Indicates enabling mining;[!badge useopencl=1] Indicates the use of GPU for mining.[!badge opencldevice=] Name of the OpenCL device to use (defaults to first available).

```
mineaddress=
mine=1
useopencl=1
opencldevice=
```
> Currently, one node only supports mining with one GPU.

## Monitor your miner

You can monitor your miner by reviewing the logs in the terminal. Theses logs provide real-time updates on your miner's status, including whether you have found a block, if it has been accepted or rejected, and your current hashrate.