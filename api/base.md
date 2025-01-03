---
icon: file
order: 1000
---
# How to CLI

!!!
Currently, the CLI tool supports most Bitcoin RPC instructions. Please check the API guide for specific details.
!!!

(CLI) is the command line interface tool of the Marscoin , you can use the command line in the terminal to interact with the node. This is useful for users who prefer to use a terminal or for servers without a graphical interface.

The `--help` option can be passed with any command to get additional details, for instance `Marscoin.Cli --help` will return all options for the `Marscoin.Cli` command.

The command `Marscoin.Cli --version` will return the current version number of your Marscoin install. See all public Marscoin.Cli [JSON RPC].

Let's go through each of the `Marscoin.Cli` CLI commands and be sure to check out the [Getting Started](/guides/configuration.md) guide for step-by-step instructions on using each of these commands.

```shell Marscoin.CLI
Usage:
 dotnet run <Marscoin..Cli/Marscoin.Cli.dll> [options] <command> [arguments]

Command line arguments:

[options]                          Options for the CLI (optional) - e.g. -help, -rpcuser, see below.
[command]                          Name of RPC method.
[arguments]                        Argument by position (RPC) or Name = Value pairs (API) (optional).

Options:
-help                              This help message
-rpcconnect=<ip>                   Send commands to node running on <ip> (default: 127.0.0.1)
-rpcport=<port>                    Connect to JSON-RPC on <port> (default for Marscoin: 33334 or default for Bitcoin: 8332)
-rpcuser=<user>                    Username for JSON-RPC connections
-rpcpassword=<pw>                  Password for JSON-RPC connections

Examples:
dotnet run Marscoin.Cli -rpcuser=admin -rpcpassword=123456 -rpcconnect=127.0.0.1 -rpcport=26174 getinfo - Displays general information about the Stratis node on the 127.0.0.3:26174, authenticating with the RPC specified user.
```

!!!
All configurations are optional. If a config is not set, Marscoin CLI will use default values.
!!!