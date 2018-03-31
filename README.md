# Tic-Tac-Toe Game on the Ethereum Blockchain!

Taken from this [Udemy course](https://github.com/tomw1808/blocktactoe)

## Initial setup (for new projects)

Unbox a new [Truffle Box](http://truffleframework.com/boxes/). In this example we will use the [Truffle Webpack Box](http://truffleframework.com/boxes/webpack).

`truffle unbox webpack`

## Useful commands

Here are some of the most common and useful commands that you will run in a typical Truffle project:

Compile: `truffle compile`
Migrate: `truffle migrate`
Test: `truffle test`
Console: `truffle develop`
Lint: `npm run lint`
Dev: `npm run dev`
Build: `npm run build`

## Run tests

To run tests you can open a development console (using `truffle develop`) and then run the command `test`.

## Start development

To start development you need to open two consoles. In one console run:

`truffle develop`

In the second console run:

`npm run dev`

## Meta Mask and the Rinkeby Test network

Install the Meta Mask Firefox plugin then either create a new account or login.

Then you can get some Ether from the Rinkeby Faucet by visiting [rinkeby.io](rinkeby.io) and clicking on the [crypto faucet link](https://www.rinkeby.io/#faucet).

## Connect Meta Mask to private Truffle development blockchain

Open Meta Mask and select 'Custom RPC' from the networks dropdown.

Enter the network address (which is output when you run `truffle develop`) and save it.

Then you can send Ether to the Meta Mask wallet via the Truffle console by running the following  command:

`web3.eth.sendTransaction({from: web3.eth.accounts[0], to: 'META-MASK-WALLET-ADDRESS', value: web3.toWei(1, 'ether')})`