---
icon: file
label: Node
---
# Node API

You can use this API to interact with a wallet, check the balance, or build a transaction.
It contains all the necessary methods for developing an application or integrate Marscoin into your system.

### Methods
---

#### `getinfo`

Gets general information about the full node.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getinfo
```

#### `getblockcount`

Gets the current consensus tip height.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getblockcount
```

#### `getblockheader`

Gets the block header of the block identified by the hash.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getblockheader {hash}
```

#### `validateaddress`

Returns information about a bech32 or base58 bitcoin address.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 validateaddress {address}
```

#### `getblock`

Returns the block in hex, given a block hash.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getblock {blockHash}
```

#### `getnetworkinfo`

Returns an object containing various state info regarding P2P networking.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getnetworkinfo
```

#### `getblockchaininfo`

Returns an object containing various state info regarding blockchain processing.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getblockchaininfo
```

#### `addnode`

Adds a node to the connection manager..{command}:add,remove,onetry

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 addnode {ip} {command}
```

#### `getpeerinfo`

Gets peer information from the connection manager.

```
Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=332 getpeerinfo
```