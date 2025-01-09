---
icon: file
label: Wallet
---

# Wallet API

You can use this API to interact with a wallet, check the balance, or build a transaction.
It contains all the necessary methods for developing an application or integrate Martiscoin into your system.


### Methods
---

#### `createwallet`

Creates a new wallet on this full node.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 createwallet {walletname} {password}
```

#### `sendtoaddress`

Sends money to an address. Requires wallet to be unlocked using walletpassphrase.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 sendtoaddress {address} {amount}
```

#### `setwallet`

Selects the active wallet on RPC based on the name of the wallet supplied.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 setwallet {walletname}
```

#### `getnewaddress`

Returns a new wallet address for receiving payments.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getnewaddress
```

#### `getbalance`

Gets wallets spendable balance.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getbalance
```

#### `gettransaction`

Get detailed information about an in-wallet transaction.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 gettransaction {txid}
```

#### `sendmany`

Creates and broadcasts a transaction which sends outputs to multiple addresses.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 sendmany {fromAccount} {addressesJson}
```

#### `getwalletinfo`

Provides information about the wallet.

```
Martiscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 getwalletinfo
```