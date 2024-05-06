# Solidity Vault and ERC20 Token Contract
This repository contains two Solidity contracts: Vault and ERC20. Below is a brief description of each contract:

# Vault Contract
The Vault contract is designed to manage the deposit and withdrawal of ERC20 tokens in a secure and efficient manner. It includes functionalities such as depositing tokens, withdrawing tokens, and managing the total supply and individual balances of the deposited tokens.

# Functions:
1. deposit(uint _amount) external: Allows users to deposit ERC20 tokens into the vault, minting corresponding shares to the depositor.
2. withdraw(uint _shares) external: Enables users to withdraw deposited tokens from the vault by burning the specified amount of shares.
# Features:
1. Implements the ERC20 interface with totalSupply, balanceOf, and allowance.
2. Ensures secure token transfers using transferFrom and transfer functions.
3. Optimizes token deposit and withdrawal by calculating shares based on the total supply and token balances.
# ERC20 Token Contract
1. The ERC20 contract is a basic implementation of the ERC20 token standard. It provides functionalities for transferring tokens, approving token transfers, and managing allowances. Additionally, it includes functionalities for minting and burning tokens.

# Functions:
1. transfer(address recipient, uint amount) external: Transfers tokens from the sender's account to the recipient's account.
2. approve(address spender, uint amount) external: Approves the spender to spend a specified amount of tokens on behalf of the owner.
3. transferFrom(address sender, address recipient, uint amount) external: Transfers tokens from one account to another, approved by the owner.
4. mint(uint amount) external: Mints new tokens and adds them to the total supply.
5. burn(uint amount) external: Burns tokens from the sender's account and subtracts them from the total supply.

# Features:
Implements the ERC20 standard interface with totalSupply, balanceOf, allowance, and event emissions.
Provides functionalities for minting and burning tokens, allowing for controlled token supply adjustments.
