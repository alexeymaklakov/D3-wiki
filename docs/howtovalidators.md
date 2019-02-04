# Validator's processes

## Set up

To perform the functions D3 **_Validators_** should:

1.	Install and configure [**_D3 validation node_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/nodes.md "Nodes in D3 network") according to the [**_manual_**] (for validating internal D3 transactions)

2.	Install and configure **_Bitcoin blockchain node_** (for validating cross-chain operations with Bitcoin)

3.	Install and configure **_Ethereum blockchain node_** (for validating cross-chain operations with Ethereum and ERC-20 tokens)

4.	Ensure the nodes are up and running

5.	Ensure that the nodes have access to network

6.	Ensure the nodes are not manipulated or modified by third parties except for the agreed process of nodes maintenance and updates by the [**_Operator_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/operator.md "Operator").

## Validation process

A **_transaction_** is considered **_valid_** if it has a correct format according to validation rules, and its application does not violate rules about global state of the blockchain.

A transfer transaction from one **_D3 Account_** to another has to be validated against the following criteria:

1.	An amount is a positive number and asset precision is consistent with the asset definition
2.	Source account has enough amount of asset to transfer and it is not zero
3.	Source account can transfer money, and destination account can receive money (their roles have these permissions)

All the checks are handled automatically by **_D3 Validation node_** and do not require manual processing.

If a transaction passes all the validation checks then it is included in a block.

For detailed technical information regarding the Validators role please refer to **_Yet Another Concensus Protocol (YAC)_** [**_description_**](https://arxiv.org/pdf/1809.00554.pdf "Yet Another Concensus Protocol").
