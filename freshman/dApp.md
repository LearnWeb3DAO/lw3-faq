# dApp
Q1. How to connect to a testnet other than Ropsten on Level 7 of Freshman Track?
The Level 7 Freshman Track under the heading "Connect Your Webpage to Your Smart Contract" Item 3 - The code in the index.html is:
const provider = new ethers.providers.Web3Provider(window.ethereum, "ropsten");
To connect to any network that the wallet (metamask) is already connected to, please drop the value of the network i.e "ropsten" from the code. So the code should read like: const provider = new ethers.providers.Web3Provider(window.ethereum);
The above will allow you to connect to whatever test network you are on and interact with the defined contract!
