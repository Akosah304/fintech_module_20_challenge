# fintech_module_20_challenge

## Background

In order to automate the formation of joint savings accounts and enable the deposit and withdrawal of funds, create a Solidity smart contract that takes two user addresses.

## Technologies

This project uses the following packages:

* [Remix](https://remix.ethereum.org/) - Remix is an IDE and compiler that runs in the browser that lets users debug transactions and create Ethereum contracts using the Solidity programming language..

* [Solidity](https://docs.soliditylang.org/) - Solidity is a high-level, object-oriented language used to create smart contracts. Programs known as "smart contracts" control how accounts behave in the Ethereum state.


## Installation Guide

You can work on this project online. No packages need to be installed locally.


## Usage

Please download the project or clone the project using git clone

Please launch remix by typing the following on the browser:

```python
https://remix.ethereum.org/
```

---

## Set up accounts

1.Remix VM (London) - This indicates the environment in which your smart contract is being executed, specifically the Remix virtual machine configured for the London network.

2. **Account**: The Ethereum address (0x5B3...eddC4) associated with the current account, along with its balance. 
 
3. **Gas Limit**: The maximum amount of gas (3000000) allocated for executing transactions. Gas is a unit used to measure the computational effort required to execute operations on the Ethereum network. 
 
4. **Value**: The value of Ether (0 Wei) being sent with the transaction.
 
5. **Contract**: JointSavings - A smart contract named JointSavings deployed from the file joint_savings.sol. It's a Solidity contract designed to automate the creation of joint savings accounts, accepting two user addresses.


6. **Transactions Recorded**: Information about recorded transactions, including the transaction hash, block hash, block number, sender address, gas used, transaction cost, input data, and decoded input. 
      
7. **Status**: Indicates the status of the transaction, whether it was successfully mined and executed. 

This information provides details about the deployment and execution of smart contracts using Remix on the Ethereum network, particularly in the London environment.

**Add 2 joint accounts to the contract**

Account 1: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb

Account 2: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0


![Set Account](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/set_account%201.png)


![Set Account 2](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/set_account%202.png)


## Deposit 1 ether

1. **[vm]**: Indicates that the transaction occurred within the Remix virtual machine. 
 
2. **from**: The sender's Ethereum address (0x5B3...eddC4). 
 
3. **to**: The recipient's contract address (JointSavings.deposit()). 
 
4. **value**: The amount of Ether sent with the transaction (1000000000000000000 Wei, equivalent to 1 Ether).

5. **status**: Indicates the status of the transaction, confirming that it was successfully mined and executed. 

6. **transaction hash**: A unique identifier for the transaction (0xdaf6b6b290dfa142a20855e8cd21505f561e339c823c663890591eaf9d427a46). 
 
7. **block hash**: The hash of the block in which the transaction was included (0x0faed680d1e8e2dd59aed5fe5a431663f4229f7db420e1e82a6ba37a7dda2bac). 
 
8. **gas**: The amount of gas used for the transaction (49871 gas). 
 
9. **transaction cost**: The total cost of the transaction (43366 gas). 
 
10. **execution cost**: The cost of executing the transaction's code (22302 gas). 
 
11. **value**: The value transferred with the transaction (1000000000000000000 Wei). 

The following logs detail a transaction where Ether was sent from one address to a contract address, executing the deposit function of the JointSavings contract, with specific gas usage and cost metrics provided.

Sender Account = 0x5B3....eddc4

Sender Account balance = 100 (before deposit) 

1 ether (deposit amount) - gas = 98.999...

Recipient Account = JointSavings

![Deposit 1 Ether](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/deposit_1_ether.png)

1. **Balance: 1 ETH**: Indicates the current balance of 1 Ether in the contract. 

2. **deposit**: Likely a function within the smart contract allowing users to deposit Ether into the joint savings account.
 
3. **contractBalance**: Potentially a function to check the balance of the contract.
   
Balance: 0 ETH (before deposit) + 1000000000000000000 Wei (deposit amount) = 1 ETH

ContractBalance: 1000000000000000000 Wei

![Deposit 1 Ether 2](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/deposit_1_ether..png)


## Deposit 10 ether

Balance: 1 ETH (before deposit) + 10000000000000000000 Wei (deposit amount) = 11 ETH

ContractBalance: 11000000000000000000 Wei

![Deposit 10 Ether](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/depsoit_10_ether.png)

Sender Account = 0x5B3....eddc4

Sender Account balance = 100 (before deposit) 

10 ether (deposit amount) - gas = 89.999...

Recipient Account = JointSavings

![Deposit 10 Ether 2](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/deposit_10_ether..png)


## Deposit 5 ether
Balance: 11 ETH (before deposit) + 5 ETH (deposit amount) = 16 ETH

ContractBalance: 16000000000000000000 Wei

![Deposit 5 Ether](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/deposit_5_either.png)

Sender Account = 0x5B3....eddc4

Sender Account balance = 100 (before deposit) - 5 ether (deposit amount) - gas = 94.999...

Recipient Account = JointSavings

![Deposit 5 Ether 2](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/deposit_5_ether..png)


## Withdraw 5 ether into Account 1
Balance: 16 ETH (before widthdrawal) - 5 ETH (withdrawal amount) = 11 ETH

ContractBalance: 11000000000000000000 Wei

Last to Withdraw Account = 0x0c066... (updated to joint account #1)

Last to Withdraw Amount = 5000000000000000000 (updated to 5 Ether)

![Withdraw 5 Ether account 1](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdraw_5_ether_account_1.png)


### last to withdraw
![Withdraw 5 Ether last to withdraw](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdraw_5_ether_last_to_withdraw.png)


### last withdraw amount
![Withdraw 5 Ether last withdraw amount](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdarw_5_ether_last_withdraw_amount.png)


## Withdraw 10 ether into Account 2
Withdrawal 10 Ether

Balance: 11 ETH (before widthdrawal) - 10 ETH (withdrawal amount) = 1 ETH

ContractBalance: 1000000000000000000 Wei

Last to Withdraw Account = 0x7A... (updated to joint account #2)

Last to Withdraw Amount = 10000000000000000000 (updated to 10 Ether)

![Withdraw 10 Ether](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdraw_10_ether_account_2.png)


### last to withdraw
![Withdraw 10 Ether last to withdraw](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdraw_10_ether_last_to_withdraw.png)


### last withdraw amount
![Withdraw 10 Ether last withdraw amount](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdarw_10_ether_last_withdraw_amount.png)

### Withdrawal Ether Without Sufficient Funds

Attempt to send 2 Ether to an account address (0x583..., valid joint account) with insufficient funds (contract only has 1 Ether Balance)

Balance: 1 Eth (unchanged)

Last to Withdraw Account = 0x988...(different account)

Last to Withdraw Amount = 10000000000000000000 (Unchanged)

![Withdrawal Ether Without Sufficient Funds](https://github.com/Akosah304/fintech_module_20_challenge/blob/main/Starter_Code/Execution_Results/withdarwal%20amount%20error.png)