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
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 createwallet {walletname} {password}
```

#### `sendtoaddress`

Sends money to an address. Requires wallet to be unlocked using walletpassphrase.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 sendtoaddress {toaddress} {walletpassword} {amount}
```

#### `setwallet`

Selects the active wallet on RPC based on the name of the wallet supplied.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 setwallet {walletname}
```

#### `getnewaddress`

Returns a new wallet address for receiving payments.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 getnewaddress
```

#### `getbalance`

Gets wallets spendable balance.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 getbalance
```

#### `gettransaction`

Get detailed information about an in-wallet transaction.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 gettransaction {txid}
```

#### `sendmany`

Creates and broadcasts a transaction which sends outputs to multiple addresses.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 sendmany {fromAccount} {walletpassword} {addressesJson}
```

#### `getwalletinfo`

Provides information about the wallet.

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=19332 getwalletinfo
```