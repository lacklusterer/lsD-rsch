# What is Lista DAO?

- Decentralized liquidity pool on BNB chain
- Earn yield from collateralized assets
- MakerDAO with modifications
- Dual token:
	* lisUSD: "destable" coin - a "new" type of stable coin
	* LISTA governance token, utility, not designed to be a "currency"

- Earn yield with 2 primary ways: liquidity staking and over-collateralized
debt positions.

# Why lista dao?

## Some defi:

- Destable coin lisUSD : [click me](https://github.com/lacklusterer/lsD-rsch/blob/main/README.md#destable-coin)
- Price stability: [click me](https://github.com/lacklusterer/lsD-rsch/blob/main/README.md#lisusd-price-stability) (minor, maybe only need to talk about and don't need dedicated slide)
- Liquidity staking and restaking: [click me](https://github.com/lacklusterer/lsD-rsch/blob/main/README.md#liquid-staking-tokens-lsts) 
- AMO: [official docs](https://docs.bsc.lista.org/introduction/collateral-debt-position/lisusd/algorithmic-market-operations-amo) 
	* dynamic lisUSD destable coin borrow rate, similar to crvUSD MonetaryPolicy from curve finance
![formula](https://docs.bsc.lista.org/~gitbook/image?url=https%3A%2F%2Flh7-us.googleusercontent.com%2Fdocsz%2FAD_4nXfRbturnppWrw7w0t-PLXhA2vzUoiV-iNor96k0jyzwnkHgvWjGfpEo85koiXXrodJJdSlZKPgDfYANjMgBFRgzIrQuoNqbLL_m6Ku7XoCEPIUOFU2D6hvjwJTgzzcDyMAEoIlnBlIy4fW_S2m7_Dwghk5v%3Fkey%3Dqpnu5MtZ54GEwy9P7UA52A&width=300&dpr=1&quality=100&sign=c7ed55e5&sv=1)

- `r0`: default annual rate, different for each collateral
- `beta`: adjustment value
	* these have large impact on price, set on the launch of contract, later community-voted
- calculates borrow rate in real time: every 15 minutes or when user take out a loan / repay

ex:
r0 = 8%, Price(lisUSD) = $0.98, Beta = 2%
r = 8% * exp[(1 - 0.98)/2%] = 21.746% 

This means if the price of lisUSD is $0.98, with  r0 = 8%  and Beta = 2% , the current borrowing rate will be 21.746%. Users will repay (burn) lisUSD, reducing the supply.

## why lista dao

- over-collateralized stable coin and liquidity staking are successful model
tried-and-true by MakerDAO:
	* increased capital efficiency: Capital are not "dead/frozen" once put down
	and still can be utilized in other DeFi protocols to maximize yield
	* mechanisms to ensure the health of the pool, liquidity and stability
		+ destable coin, liquidation in dutch auction

- [This space is for section "Participating entities incentives"]

# Additional readings:

https://www.gate.io/learn/articles/introduction-to-lista-dao/3382

https://docs.bsc.lista.org/
