# - - - - - - C H A I N  L I N K - - - - - -

### uses of ChainLink

**i.    datafeeds** - uses ofchain data like price os ETH in USD.
**ii.    Randomization** - Generate random number which is completely random.
**iii.    Automation** - to automate some functionalities in the smartcontracts.
**iv.    API calls** - offchain api calls.


### 1. ChainLink Automation

its helps to automate a specific function in a smart contract..

*Steps to automate any functionality in the contract are given below.*

1. Open the Chainlink Automation app from this link. `https://automation.chain.link/?_ga=2.127831631.356220654.1672857615-371040361.1670998780`
2. Register a new Upkeep.
3. SElect Time based trigger.
4. Specify time schedule.
5. fund the upkeep with **link tokens.**
7. paste the smart contract address and ABI in chainlink.(if required)
6. done.

`You can also change the upkeep status in future like fund more tokens, stop or update with 'automation.chain.link' webapp `


### 2. ChainLink Datafeed

*Steps to add Datafeed functionality in the solidity contract are given below.*

1. import AggregatorV3Interface.sol in to the contract

`import "@chainlink/contracts/src/v0.8/interfaces/AggregatorV3Interface.sol";`

2. in constructor inicialize a variable with aggregatorV3Interface interface by using "0xD4a33860578De61DBAbDc8BFdb98FD742fA7028e" this address.

*Important*

 ```
Network: Goerli
Aggregator: ETH/USD
Address: 0xD4a33860578De61DBAbDc8BFdb98FD742fA7028e
```

3. call functions of that interface to fetch different prices data.


### 3. ChainLink Randomization

its helps to generate truly random data.

*Steps to Generate any data in the contract are given below.*

1. check if you are enough eth and Link Tokens in your Metamask.
2. Open the Subscription Manager at vrf.chain.link.
3. Create Subscription
4. add Funds in to this Subscription
5. After you add funds, click Add consumer. A page opens with your account details and subscription ID.
6. while deploying smart contract in constructor specify your subscriptionId so the constructor can set it.
7. paste the smart contract address and ABI in chainlink.