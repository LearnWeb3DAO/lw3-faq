# Whitelist


### Q) I was able to compile the contract but while deploying I was running into the following error. 
ReferenceError: deployedWhitelistContract is not defined
    at main (/home/user/Documents/web3_Learning/web3_learning/web3_learning/new/web3_learning/Whitelist-Dapp/scripts/deploy.js:11:46)
    at processTicksAndRejections (internal/process/task_queues.js:97:5)
what am i doing wrong?

-Make the sure you store the response from the deployed() method and then try to access the contract address. Make the following changes in the code:
const deployedWhiteListResp = await deployedWhiteListContract.deployed();
console.log("Whitelist Contract Address:", deployedWhiteListResp.address);
