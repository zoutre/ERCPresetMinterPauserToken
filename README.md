# ERCPresetMinterPauserToken
Starting point for initial token creation contract.

# OpenZepplin GitHub import
<!--- myToken.sol full example logic --!>
```
    pragma solidity >=0.7.0 <0.9.0;
    import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/presets/ERC20PresetMinterPauser.sol";
    contract myToken is ERC20PresetMinterPauser {
        constructor() ERC20PresetMinterPauser("myToken", "MINE") {
        }
    }
```
