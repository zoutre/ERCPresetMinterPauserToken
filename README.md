# ERCPresetMinterPauserToken
Starting point for initial token creation contract.

# Development
<!--- myToken.sol full example logic --!>
```solidity
pragma solidity >=0.7.0 <0.9.0;
import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/presets/ERC20PresetMinterPauser.sol";
contract myToken is ERC20PresetMinterPauser {
    constructor() ERC20PresetMinterPauser("myToken", "MINE") {
    }
}
```
## Token creation
Openzepplin: https://docs.openzeppelin.com/contracts/3.x/api/presets#ERC20PresetMinterPauser

## Upgradable contract (e.g., no constructor())
Openzepplin: https://docs.openzeppelin.com/upgrades-plugins/1.x/writing-upgradeable
