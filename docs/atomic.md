# Atomic exchange between D3 Clients

**_Atomic exchange_** allows to make trustless swap with two counterparts.

A direct exchange requires two transactions to be made. The problem is that one of (or both) the participants may not follow the deal protocol and make no (or wrong) transactions. 

**_Atomic exchange_** ensures that all the agreed transactions are either processed all together, or not processed at all. All the transactions are packed into a batch and this batch passes necessary validations and only if all of them are successful the batch is processed.

