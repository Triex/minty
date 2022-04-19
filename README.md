# minty

Minty is an example of how to _mint_ non-fungible tokens (NFTs) while storing the
associated data on IPFS. You can also use Minty to pin your data on an IPFS pinning service such as [nft.storage](https://nft.storage) and [Pinata](https://pinata.cloud). 

## Usage

Run `minty help` to see full usage instructions or `minty help <command>` for help on a specific command: 

```shell
minty help mint

> create a new NFT from an image file
> 
> Options:
>   -n, --name <name>         The name of the NFT
>   -d, --description <desc>  A description of the NFT
>   -o, --owner <address>     The ethereum address that should own the NFT.If not provided,
>                             defaults to the first signing address.
>   -h, --help                display help for command
```

## Setup 

To install and run Minty, you must have NPM installed. Windows is not currently supported.

1. Clone this repository and move into the `minty` directory:

    ```shell
    git clone https://github.com/yusefnapora/minty
    cd minty
    ```

1. Install the NPM dependencies:

    ```shell
    npm install
    ```

1. Add the `minty` command to your `$PATH`. This makes it easier to run Minty from anywhere on your computer:

    ```
    npm link
    ```

1. Run the `start-local-environment.sh` script to start the local Ethereum testnet and IPFS daemon:

    ```shell
    ./start-local-environment.sh

    > Compiling smart contract
    > Compiling 16 files with 0.7.3
    > ...
    ```

    This command continues to run. All further commands must be entered in another terminal window.

