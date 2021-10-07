# Aragon Hardhat Configuration file

## Install

```
$ npm install --save-dev @aragon/hardhat-config
```

And add the following statement to your hardhat.config.js:

```
module.exports = require('@aragon/hardhat-config')
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

By supplying `--network <network>` to a [hardhat](https://hardhat.org) command, it will use the private key and url setup for that network in the `<network>_key.json` file.

