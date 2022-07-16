local eth

foundry docs: [foundrybook](https://book.getfoundry.sh/)
sol scripting: [boo](https://book.getfoundry.sh/tutorials/solidity-scripting)

env

```env
RINKEBY_RPC_URL=
PRIVATE_KEY=
ETHERSCAN_KEY=
```

start

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

edit .sol then

```bash

forge build

... compiler build success

```

run script

```bash

# To load the variables in the .env file
source .env

# To deploy and verify our contract
forge script script/NFT.s.sol:MyScript --rpc-url $RINKEBY_RPC_URL  --private-key $PRIVATE_KEY --broadcast --verify --etherscan-api-key $ETHERSCAN_KEY -vvvv

```

:sunglasses: :v:
