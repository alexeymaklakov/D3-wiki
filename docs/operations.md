# Operations supported in D3ledger

### Crypto Assets Deposit

When a [**_Client_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") wants to deposit a crypto asset to **_D3 account_** he/she should send the asset to a dedicated account on original asset blockchain. 

Once received the asset is “locked” on the original blockchain and an equivalent token is released on the **_D3ledger client account_**. After that the [**_Client_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") can operate crypto asset on D3ledger. 

### Crypto Assets Withdrawal

[**_Client_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") can withdraw crypto assets at any time.  When the transaction passes security validations the specified asset amount is “unlocked” on the primary blockchain and transferred to the account, specified by the client.

### Crypto Assets Transfer to other D3 Clients

D3ledger enables assets transfer between [**_Clients_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") in a fast and cost-effective way. Transfer of assets in D3ledger remains fast, reliable and private as it does not require transactions in native blockchains. D3ledger transfers take just several seconds to be processed (in case of transaction in native blockchains it may take more than one hour to process and require transaction fees may vary dramatically depending on the transaction queue size).

### Crypto Assets Exchange

[**_Clients_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients in D3 network") can exchange assets with each other inside D3 platform directly. The exchange includes two participants and two assets. 
Once the participants agree on the amounts they initiate a direct exchange. D3 uses an [**_Atomic exchange_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/atomic.md "Atomic exchange between D3 clients") algorithm to ensure the exchange participants follow the exchange protocol.


 
