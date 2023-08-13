# Reading 49 Forward Commitment and Contingent Claim Features and Instruments

## 1. Forward and Futures

- Forward contracts: last Reading has mentioned
- Future contracts
  - similar to Forward Contract, but is <u>standardized and exchange-traded</u>(secondary market) 
  - backed by Central Clearinghouse(CCH), required daily cash settlement of gain/loss, minimizing counterparty credit risk
  - **margin**:
    - cash or 或者其他可抵押物, both buyer&seller must deposit
      - 抵押物provide protection for clearinghouse
    - no involved loan, no interest charges
    - **marking to market**: 每天结束, margin balance of future is adjusted for any gains/loss in position based on new <u>settlement price</u>.
      - settlement price calculation: <u>average prices of trades</u> at the end of the trading session
    - **Initial margin**:
      - 在trade开始之前，必须deposit在future account里的抵押物数目
      - per contract的数量is low, 约等于one day's max <u>expected price fluctuation</u> on total value of assets
    - **Maintenance Margin**: minimum amount of margin must be kept in account
      - if account balance < maintenance margin, the corresponding party should deposit additional amount until his account balance=*initial margin*，而不是maintenance one
      - if it is failed to maintain, the future position will be *closed out*.
      - it is set by the exchange.
  - price limits:
    - set by exchange
    - limit on how much each day's settlement price can change from previous day's.
    - *outside the price limit* execution is prohibited.
    - circuit breakers: when price reaches the price limits, trading is *suspended for a short period*.

## 2. Swaps and Options

- Swaps
  - Definition:
    - exchange a *series of payment* on *multiple settlement dates* over a period of time
    - on the payment date, two payments from counterparty are offset-->only *one net payment* is made
  - counterparty risk:
    - trade in dealer market
- Credit Swaps
- Options
- forward commitment:
  - legally binding promise to do actions in future
  - content: forward contract, future contract, most swap
- contingent commitment:
  - claim/payoff depends on a particular event
  - content: options(underlying being above or below the exercise price), credit default swap(CDS)(trigger by credit default)
