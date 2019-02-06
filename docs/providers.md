# Services provided by third parties

D3ledger ecosystem enables third parties to provide various services for **_D3 clients_** extending their opportunities. For example, such services may include the following:
  
  •	Crypto currency exchange for trustless trade
  
  •	OTC brokers, who can connect to D3 through a special gate


**_Providers_** get access to **_D3Ledger_** through [**_Agents_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/agents.md "Agents of D3") and provide value added services to [**_Clients_**](https://github.com/alexeymaklakov/D3-wiki/blob/master/docs/clients.md "Clients of D3").

### External liquidity providers

D3 Ledger platform enables access to different liquidity providers to allow clients make exchange deals. 
All the providers connected to D3 agree to work on Delivery Versus Payment (DvP)  settlement form. It means that the liquidity provider can withdraw client’s assets only along with delivering another asset specified by the deal.

### External crypto exchanges gateway

External exchanges can connect to D3ledger through a special gateway. Clients’ asset security measures require trustless trade. It means that clients’ assets are not transferred to an exchange until trade settlement is processed. 

To shorten the settlement time external exchanges will be incentivized to have sufficient amount of each tradable assets in D3. 

External crypto exchange gateway allows **_Clients_** to transfer assets to a special trade account, related to a certain exchange. 

Exchange can see the assets and has the permission to transact from this account. When the exchange sees asset amount on the account, it unlocks the same asset amount on exchange trade account for the **_Client_**. 

Trades will be available only on assets supported by D3 Ledger.

### OTC Deals support

D3ledger **_Clients_** can get access to a network of OTC brokers to get the best available exchange offers on OTC-market. 

**_Clients_** post order or requests quotation for an interesting exchange to his **_Agent_**.

**_Agent_** transfers the request to a network of OTC brokers, connected to D3. 

When OTC-brokers provide their proposal a **_Client_** chooses the best one and initiates deal.

D3ledger locks **_Client_** assets for deal and awaits delivery by OTC-broker. 

On delivery client’ asset (locked for deal) are transferred to OTC Broker. 

D3ledger performs settlement functions to support the deal. From client’s view the deal happens between him and the **_Agent_**. From Agent’s view two deals happen: one with client and one with OTC-Broker. 


