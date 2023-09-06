# Module_20

# Joint Savings Account Smart Contract README

This README provides my step by step process to create, compile, deploy, and interact with a Joint Savings Account smart contract using Solidity and the Remix IDE.

## Step 1: Create a Joint Savings Account Contract in Solidity

1. Open the Remix IDE and create a new Solidity file named `joint_savings.sol` (in the Starter_Code Folder).

2. Define the `JointSavings` contract and declare the following variables:
   - `address payable accountOne`
   - `address payable accountTwo`
   - `address public lastToWithdraw`
   - `uint public lastWithdrawAmount`
   - `uint public contractBalance`

3. Define the `withdraw` function:

4. Define the `deposit` function:

5. Define the `setAccounts` function:

6. Add a fallback function to receive ether:

## Step 2: Compile and Deploy Your Contract in the JavaScript VM

1. Compile your smart contract in Remix IDE. Make sure there are no errors.

2. In the "Deploy & Run Transactions" pane, select "JavaScript VM" as the environment.

3. Click the "Deploy" button to deploy your smart contract. Confirm the successful deployment.

## Step 3: Interact with Your Deployed Smart Contract

1. Set authorized Ethereum addresses using the `setAccounts` function.

2. Test deposit functionality:
   - Send 1 ether as wei (Transaction 1)
   - Send 10 ether as wei (Transaction 2)
   - Send 5 ether (Transaction 3)
   After each transaction, verify the updated `contractBalance`.

3. Test withdrawal functionality:
   - Withdraw 5 ether into `accountOne`.
   - Withdraw 10 ether into `accountTwo`.
   After each withdrawal, use the `contractBalance`, `lastToWithdraw`, and `lastWithdrawAmount` functions to verify results.
