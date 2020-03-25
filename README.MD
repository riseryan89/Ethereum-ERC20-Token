# Ethereum ERC20 Token Contract FOR WHOM JUST BEGINS
-----------------------
### How to use:
  1. Go to <https://remix.ethereum.org/>
  2. Select Solidity for your environment
  3. Upload File you just downloaded from this repo
      - For your own mainnet, Choose Web3 Provider and type your RPC Address
  4. Select MainToken.sol
  ```solidity
      // You need to customize things.
      constructor () public ERC20Detailed("Your Token Name", "YTN", 8) { // Your Token Name, abbreviation, Decimal
        _mint(_msgSender(), 10000 * (10 ** uint256(decimals())));        // Initial Mint 10000 Token to Contract Owner
  ```
  5. Select compiler (like, 0.5.0+commit.1d4f565a)
  6. Click Compile Button
  7. Select 'Injected Web3' as your Deployment Environment
        - For your own mainnet, Choose Web3 Provider and type your RPC Address
  8. Login your Metamask
  9. Make sure the compiled file selected before Go
  10. DEPLOY!
  
### Is this Safe?
This has been FULLY audited by ME and one of the famous Smart Contract Audit Companies.
  - FIXED : Latest Big Issue Regarding unaccessibility to Transfer Function from ERC20 Contract (like USDT and 130 more)
```solidity
    function transfer(address recipient, uint256 amount) public returns (bool) {
        _transfer(_msgSender(), recipient, amount);
        return true;
    }
```
### Who I AM?
Smartcontract Composer
Any Issues, Please let me know.
Thanks for 'Fork' and 'Star'

Individual Contact to <rise.ryan.lee@gmail.com>


### What You Need to Know
This contract is issuing tokens unlimitedly.
