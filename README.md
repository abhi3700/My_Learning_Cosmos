# My_Learning_Cosmos

Learn everything about Cosmos Blockchain

## Installation

### CLI

1. Rust
2. target: `wasm-unknown-unknown`
3. `wasmd` (backbone for CosmWasm)

   > following is the guide for install/upgrade `wasmd` on macOS

   1. pre-requisites:
      1. make: `brew install make`
      2. `Go`: `brew install golang`

   ```bash
   git clone https://github.com/CosmWasm/wasmd.git
   cd wasmd
   # If you are updating wasmd, first update your local repository by fetching the remote tags available
   git fetch --tags
   # replace the v0.27.0 with the most stable version on https://github.com/CosmWasm/wasmd/tags (or look at `git tag`)
   git checkout v0.27.0
   make install

   # add path to your ~/.zshrc or ~/.bashrc
   export GOPATH=$HOME/go
   export GOROOT="$(brew --prefix golang)/libexec"
   export PATH="$PATH:${GOPATH}/bin:${GOROOT}/bin"

   # verify the installation
   wasmd version
   ```

For more, refer [this](https://docs.cosmwasm.com/docs/1.0/getting-started/installation).

### Networks

Here, the testnet, mainnet RPC, faucet and other useful links are provided to deploy contracts.

- **RPC**

  - Testnet
    - https://rpc.malaga-420.cosmwasm.com/status
    - https://faucet.malaga-420.cosmwasm.com/status

- **Block explorer**
  - Testnet
    - Malaga: https://block-explorer.malaga-420.cosmwasm.com/
  - Mainnet
    - ATOMScan: https://atomscan.com/

## References

- [CosmWasm Book](https://book.cosmwasm.com/)
- [Sylvia Book](https://cosmwasm.github.io/sylvia-book/index.html)
- [CosmWasm Academy](https://academy.cosmwasm.com/)
- [awesome-cosmwasm](https://github.com/CosmWasm/awesome-cosmwasm)
- [cosmwasm-std documentation](https://docs.rs/cosmwasm-std/)
- [Last version of this documentation sources before deprecation](https://github.com/InterWasm/docs/tree/archive)

### Videos

- Channels
  - [Spark IBC](https://www.youtube.com/@sparkibc8129)
