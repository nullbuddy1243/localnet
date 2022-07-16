local eth

foundry docs: [foundrybook](https://book.getfoundry.sh/)

```env
RINKEBY_RPC_URL=
PRIVATE_KEY=
ETHERSCAN_KEY=
```

```bash
$ anvil -a 10 --hardfork latest  -p 7070

                             _   _
                            (_) | |
      __ _   _ __   __   __  _  | |
     / _` | | '_ \  \ \ / / | | | |
    | (_| | | | | |  \ V /  | | | |
     \__,_| |_| |_|   \_/   |_| |_|

    0.1.0 (37e4376 2022-07-16T00:19:06.15167Z)
    https://github.com/foundry-rs/foundry


```

```bash
$ forge script script/NFT.s.sol:MyScript --rpc-url $RINKEBY_RPC_URL --private-key $PRIVATE_KEY --broadcast --verify -vvvv --etherscan-api-key $ETHERSCAN_KEY
```
