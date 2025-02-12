---
icon: terminal
tags: [guide]
order: 100
---
# Create your wallet using CLI

!!!
Currently, the CLI tool supports most Bitcoin RPC instructions. Please check the API guide for specific details.
!!!

## `Create Wallet`

The `createwallet` command is the easiest way to get your project built and running in a browser within seconds.

[!badge walletname] input your wallet name, [!badge password] input wallet password.

#### Windows

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 createwallet {walletname} {password}
```

#### Linux

```
dotnet Martiscoin.Cli.dll -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=29332 createwallet {walletname} {password}
```

The returned [!badge result] contains 12 characters, which is the wallet mnemonic,please save it.

#### Response

```
{
    "result": [
        ""
    ],
    "error": null
}
```