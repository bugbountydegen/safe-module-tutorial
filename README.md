# safe-module-tutorial

Example from https://docs.safe.global/advanced/smart-account-modules/smart-account-modules-tutorial

You will build a TokenWithdrawModule that enables beneficiaries to withdraw ERC20 tokens from a Safe account using off-chain signatures from Safe owners.

## Implementation Details
The TokenWithdrawModule allows:

* Safe owners to authorize token withdrawals via off-chain signatures
* Beneficiaries to execute withdrawals themselves without requiring Safe owner transactions

## Limitations
* Each beneficiary has a sequential nonce, requiring withdrawals to be processed in order
* The module is bound to a specific token and Safe address at deployment

## Installation
```
git clone https://github.com/bugbountydegen/safe-module-tutorial.git
cd safe-module-tutorial
npm i
npx hardhat compile
npx hardhat test
```
