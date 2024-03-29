# zoutre-beta
Starting point for initial token creation to be used with zoutre-beta DeFi dApp

# Development - myToken
<!-- myToken.sol sample example logic -->
```solidity
pragma solidity >=0.7.0 <0.9.0;
import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/presets/ERC20PresetMinterPauser.sol";

contract myToken is ERC20PresetMinterPauser {
    constructor() ERC20PresetMinterPauser("myToken", "MINE") {
    }
}
```
## Windows x64 - Tools
* PowerShell (local command-line environment)
* Notepad++ (source code viewer): https://notepad-plus-plus.org/
* GitHub (source repository and git CLI): https://github.com/
  * Using Git with GitHub: https://docs.github.com/en/get-started/using-git/about-git
* Node.js (Javascript engine): https://nodejs.org/en/
* Truffle (smart contract development / production deployment): https://trufflesuite.com/
* Infura (Web3 Provider - API): https://infura.io/
  * Using Infura with Truffle: https://trufflesuite.com/guides/using-infura-custom-provider/
  * Validate Infura account by retrieving current block number of blockchain: 
```curl
  curl https://ropsten.infura.io/v3/<Project ID> \
   -X POST \
   -H "content-Type: application/json" \
   -d '{"jsonrpc":"2.0","method":"eth_blockNumber","params":[],"id":1}'
```
  * Get unique mnemonics: `npx mnemonics` 
* Metamask Chrome extension (crypto wallet): https://metamask.io/download/ 
  * Ropsten (Ethereum-like PoW blockchain testnet): https://ethereum.org/en/developers/docs/networks/
  * ETH Faucet (test crypto): https://fauceth.komputing.org/
* Ethereum security: https://ethereum.org/en/developers/docs/smart-contracts/security/

## Token creation
Openzepplin: https://docs.openzeppelin.com/contracts/3.x/api/presets#ERC20PresetMinterPauser

## Upgradable contract (e.g., no constructor())
Openzepplin: https://docs.openzeppelin.com/upgrades-plugins/1.x/writing-upgradeable
