# Swap Token List
Token list for [swap.country](https://swap.country/).

# Adding new tokens
## The Approval process
1. Technical team will validate the input to ensure the data is matching with the expected pattern
2. Harmony team will analyze the token and project in terms of value brought into Harmony ecosystem

## Requirements and Recommendations
- One token is accepted per one pull request
- Token data must match contract data
- Token must have a logo
- PR file structure should match the existing structure of the repository (e.g. putting logos in  ```TOKEN_SYMBOL/logo.png```)
- Contract should be verified*
- Project should have a significant role in network's ecosystem
  

_*We highly recommend that the contract is verified as this will be taken into consideration during the evaluation and approval process by the Harmony team_

## Steps
- Fork this repository
- Create token folder with similar structure: ```TOKEN_SYMBOL/logo.png```. [Example](https://github.com/harmony-one/swap-token-list/tree/main/assets/WONE)
- Edit [tokenlist.json](https://github.com/harmony-one/swap-token-list/blob/main/tokenlist.json) with token data. Example: 
```sh
    {
      "chainId": 1666600000,
      "address": "0xcf664087a5bb0237a0bad6742852ec6c8d69a27a",
      "symbol": "WONE",
      "name": "Wrapped ONE",
      "decimals": 18,
      "logoURI": "https://raw.githubusercontent.com/harmony-one/swap-token-list/main/assets/WONE/logo.png"
    },
```
- Increment the version (if new token is added: minor, if existing token data is edited - patch);
```sh
   "version":{
      "major":1,
      "minor":<<x+1>>,
      "patch":0
   }
```
- Update a timestamp (UTC in ISO format)
```sh
  "timestamp":"2024-05-05T13:16:21Z"
```
- Validate that .json file is formatted correctly (with no errors)
- Create a pull request

