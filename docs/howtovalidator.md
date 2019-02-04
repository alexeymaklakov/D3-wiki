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

All the checks are handled automatically by [**_D3 Validation node_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/nodes.md "Nodes in D3 network") and do not require manual processing.

If a transaction passes all the validation checks then it is included in a block.

For detailed technical information regarding the Validators role please refer to **_Yet Another Concensus Protocol (YAC)_** [**_description_**](https://arxiv.org/pdf/1809.00554.pdf "Yet Another Concensus Protocol").

## Operations with external blockchains

[**_D3 Clients_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") can **_transfer_** crypto assets (Bitcoin, Ethereum and ERC20 Tokens) from original blockchains and back. 

Such transactions are called cross-chain transactions. 

Cross-chain transaction are enabled by a special mechanism (**_two-way peg_**) . 

[**_Validators_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/validators.md "Validators in D3 network") approve each cross-chain transaction by consensus if it passes all the **_validation checks_**.

When a [**_Client_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") wants to **_deposit_** a crypto asset to **_D3 account_** he/she should send the asset to a dedicated account on the original blockchain (Bitcoin or Ethereum). Once received the asset is “locked” on the original blockchain and an equivalent token is released on the **_D3 Ledger Client’s account_**. After that the client can operate crypto asset on **_D3 Ledger Platform_**.

**_Client_** can **_withdraw_** crypto assets from **_D3ledger_** at any time (partially or completely). A withdrawal transaction should be created and target address in the original blockchain specified. When the transaction passes security validations the specified asset amount is “unlocked” on the primary blockchain and transferred to the target address, specified by the **_Client_**.

[**_Validators_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/validators.md "Validators in D3 network") manage D3 assets on external blockchain accounts via **_multisignature mechanism_** and ensure that **_withdrawal_** operations are processed if pass necessary validation criteria.

**_D3 Ledger Ecosystem_** is designed to have no **_single point of failure_**. If one or even several validators (less than 1/3 of total number) stop operating for any reason the ecosystem remains fully functional. 
