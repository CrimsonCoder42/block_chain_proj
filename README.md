# TheCoin.js

TheCoin.js is a simple blockchain implementation using Node.js and the crypto-js library. This project is designed to help developers understand the basics of blockchain technology and how it works.

## Installation

To install TheCoin.js, please follow these steps:

1. Ensure that Node.js is installed on your machine.
2. Clone this repository to your local machine.
3. Open the terminal or command prompt and navigate to the project directory.
4. Run the command `npm install --save crypto-js` to install the required dependencies.

## Usage

To use TheCoin.js, simply import the Blockchain class from thecoin.js and create a new instance of the class. You can then add new blocks to the blockchain using the addNewBlock method.

Here's an example:

```javascript
const { Blockchain, BlockCrypto } = require('./thecoin');

let thecoin = new Blockchain();

// Adding new blocks
thecoin.addNewBlock(new BlockCrypto(1, "06/04/2021", {sender: "Alice", recipient: "Bob", amount: 100}));
thecoin.addNewBlock(new BlockCrypto(2, "06/04/2021", {sender: "Bob", recipient: "Charlie", amount: 50}));

// Checking validity
console.log(thecoin.checkValidity());
