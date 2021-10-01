# Aragon Buidler Configuration file

## Install

```
$ npm install @aragon/buidler-config
```

## Set a private key

You can configure a private key in `~/.aragon`. Create a file`<network>_key.json`(eg. `rinkeby_key.json`) with this structure:

```json
{
  "rpc": "https://<network>.infura.io",
  "keys": ["put-your-priv-key-here"]
}
```

See [set-a-private-key](https://hack.aragon.org/docs/guides-faq#set-a-private-key) for more information on how to set a private key.

By supplying `--network <network>` to a [buidler](https://hardhat.org) command, it will use the private key and url setup for that network in the `<network>_key.json` file.

