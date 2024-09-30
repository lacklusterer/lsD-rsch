> [!NOTE]
> todo: Make up some real-life equivalent of the mechanics
> Focus: Why Lista DAO, what makes it different from existing models
> What / how can Investors, Casual users, developer do with / benefit from it?

Lista DAO main focus is collateralized debt postion stable coin (CDP) and liquidity staking

## Some problems:
**Stable coin trilemma**: decentralization, price stability, or capital efficiency

### Capital efficiency
- overcollateralized stablecoins (MakerDao-like) -> Freezes funds
	* liquidity < collateral
	* cannot be used

## CDP

- Benefit from assets without having to sell (for example, selling assets to a
DEX to provide liquidity)
- "Lock" them instead, still "owning" them
- Stake assets -> borrow lisUSD
- "Doubles" the ultility of capital: Earn stake reward and still participate in
De-fi with the same capital
- May have asset liquidated if debt

### Liquid staking Tokens (LSTs)

- tokenized version of PoS: earn PoS reward without losing access to liquidity
- trade, sell, or use "capital" while they are still staked
- 1:1 ratio to staked assets

- stake BNB for slisBNB
	* Delegate BNB to ListaDao's validator
	* Validators use this BNB in PoS for reward, keeping 5%
	* Remaining 95% goes to slisBNB holder in form of slisBNB/BNB exchange rate

### Liquid restaking tokens (LRTs)

- lock LST to mint stablecoins, in a CDP
digital assets -> stake -> get LST -> use LST in restake -> LRT

## Liquidity (re)Staking

- slisBNB
- Why?
	* <u>Capital efficiency</u>
		+ Can do more stuff with the same investment (or "capital")
	* "unlocked" liquidity
		+ Can still "use" staked assets through tokenized representative
	* 

# WIP

## lisUSD price stability
- fiat peg =/= stability because fiat also fluctuate in value
- organic, "traditional" price stabilization:
- lisUSD > $1: need more supply:
	- borrowers borrow more to sell for arbitrage
	- decrease lisUSD borrow interest -> less farming reward -> less farm demand
- lisUSD < $1: need less supply:
	- borrowers buy cheap from market to pay debt
	- increase interest -> more farming reward -> less borrowing demand

## tokenomics
- **lisUSD**: minted when user deposit collateral into CeVault (lista' colateral vault) -> lisUSD enters circulation
	- also obtained by buying from brokers/exchanges or staking lisUSD
- **LISTA**: ultility token, represent governance and ultility functions
	- payment / settlement within Lista DAO between participants
	- locked to receive veLISTA -> governance

### Loan Liquidation

- ensures Lista -> Lista lisBNB -> slisBNB lisUSD -> lisUSD in pools remains
fully backed by BNB collateral.

## destable coin

- "decentralized stable coin"
- over colateralized with decentralized assets and liquidity-staked assets
- "broadly stable" instead of absolute, backed or algorithmic , similar to
"normal fiat"

## AMO

- Algorithmic Market Operation
- Similar to curve fiance monetary policies
[formula](https://docs.bsc.lista.org/introduction/collateral-debt-position/lisusd/algorithmic-market-operations-amo#the-formula-for-calculating-the-borrowing-interest-rate-r-is-as-follows)
- Borrow rate calculated dynamically based on market price (live through oracle)
	* Also affected by some parameters set in contracts
	* Set at deployment based on "market conditions", later changed through governance processes
	
