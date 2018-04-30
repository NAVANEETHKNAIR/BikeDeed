#BikeDeed

`BikeDeed.sol` is an attempt to implement the latest draft of the ERC721 standard. 

Its inheriting contract `ERC721Deed.sol` is based on the `ERC721Token` from OpenZeppelin (https://github.com/OpenZeppelin/zeppelin-solidity/blob/master/contracts/token/ERC721/ERC721Token.sol). 

*Warning:* The standard is still open for discussion, so this project should be considered work in progress. Follow the discussion here: https://github.com/ethereum/EIPs/pull/841

## About this example

BikeDeed is a first attempt at building an Ethereum Dapp.  BikeDeed leans heavily on the incredible efforts of https://github.com/nastassiasachs/ERC721ExampleDeed, https://github.com/Michael-Free/bikechain-ethwaterloo and OpenZeppelin.  Thank you!  So far only the Chrome browser is supported.

## Prerequisites
1. npm
2. Truffle
3. Git
4. Ganache
5. Chrome browser with Metamask plugin

## Dev Installation
1. git clone https://github.com/kennethhoytwoodruff/BikeDeed.git
2. npm install
3. truffle compile
4. npm run test (optional)
5. start ganache on http://localhost:8545
6. truffle migrate
7. truffle exec scripts/populatebikedeed.js
8. truffle exec scripts/displaybikes.js (optional)
9. npm run build
10. npm run server
11. Make sure you have an Internet connection and go to http://localhost:8080 with your browser.

## Tests and mocks

The tests and mocks of this repository are based on OpenZeppelin work. The directory structure is a result of the decision to install their contracts through EthPM instead of NPM.  To perform unit tests type 'truffle exec tests/test.sh'.

## TODO
1. Searching of existing Bike deeds.
2. Editiing existing Bike deeds.
3. Remove unused Node modules.
4. Better off-chain document support. Allow the user to specified proof-of-ownership using the document of his/her choice (MD5 HASH, IPFS HASH, URL).

