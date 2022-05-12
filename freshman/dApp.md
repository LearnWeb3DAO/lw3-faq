# dApp

### Q1.
- Hey when I do the first dApp, I have this error in my console : "Uncaught ReferenceError: ethers is not defined" is it related to this :" 'ethereum.enable()' is deprecated and may be removed in the future. Please use the 'eth_requestAccounts' RPC method instead." ?

- Yes, instead of using 
``` window.ethereum.enable()
    var provider = new ethers.providers.Web3Provider(web3.currentProvider, 'ropsten');
```

- Use this 
```
let provider = new ethers.providers.Web3Provider(window.ethereum, 'ropsten')
```
