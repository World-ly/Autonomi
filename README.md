# __Autonomi__

###  Exploring an ethereum based solution to enable a truly autonomous, self-governing car-sharing platform.

Functionalities are split across 3 categories

The default  [StandardToken.sol](https://github.com/ConsenSys/Tokens/blob/master/contracts/StandardToken.sol) implements the core ERC20 standard functionality [#20](https://github.com/ethereum/EIPs/issues/20). This core functionality will be shared across both human and machine platforms.



The [HumanStandardToken.sol](https://github.com/ConsenSys/Tokens/blob/master/contracts/HumanStandardToken.sol) has added functionality for human operations. It includes but is not limited to:  

1. Bid on Car Adoption Contract.
2. Basic voting functionality amongst shared car holders for conflict settlement and parts upgrading.
3. Time based contracts created by scheduler to allocate temporary car ownership dynamically


There is a set of tests written for the HumanStandardToken.sol using the Truffle framework to do so.

The [MachineStandardToken.sol](https://github.com/ConsenSys/Tokens/blob/master/contracts/HumanStandardToken.sol) has added functionality for machine operations. It includes but is not limited to:  

1. Receive bids on Vehicle Adoption Contract. Based on scheduler accepts compatible candidates and returns unsuccessful bids.
2. Machine to Machine payments that allows for retrieval of funds without human acknowledgement
3. Allow credited humans to withdraw from machine wallet to make repairs and upgrades



## Testing

```npm install```

For getting truffle-hdwallet-provider. Solidity tests have to still be written.

Uses Truffle 3.x.


## Contributing

**Pull requests are welcome!**

When submitting a pull request, please do so to the `staging` branch.

### Licensed under MIT.  

This code is licensed under MIT.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
