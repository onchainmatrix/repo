# Treasury Reporting and Performance Methodology

Onchain Matrix is designed to make treasury reporting understandable, comparable over time, and reconcilable with onchain evidence while avoiding disclosure of information that could compromise execution security.

This methodology separates capital formation, asset valuation, realized yield, unrealized market movement, protocol revenue, and treasury growth so that a single headline number does not obscure the underlying economics.

## Core reporting definitions

### Treasury Principal

Capital designated as part of the protocol-owned productive treasury base. Treasury principal is intended to be preserved, deployed, and accumulated rather than treated as routine operating cash.

### Treasury Value

The aggregate value of assets attributed to the protocol treasury at the applicable reporting timestamp, using the valuation methodology assigned to each asset category.

### Available Liquidity

Treasury assets that can be accessed or converted within the applicable liquidity policy without first exiting a longer-duration strategy or credit position.

### Deployed Capital

Treasury capital actively allocated to approved strategies, assets, RWA exposures, or credit positions.

### Realized Yield

Income or gains that have been realized through completed protocol activity, strategy distributions, interest or credit payments, staking or yield receipts, or closed positions.

### Unrealized P\&L

Changes in the marked value of open treasury positions that have not yet been realized through sale, redemption, repayment, or settlement.

### Protocol Revenue

Revenue attributable to protocol activity. Potential sources include treasury yield, credit spread participation, origination and servicing fees, and future pool or marketplace activity.

### Operating Expense

Approved protocol expenditure for infrastructure, security, development, liquidity support, operations, and ecosystem activity.

### Net Revenue Retained

Protocol revenue remaining after the applicable operating costs and other approved revenue allocations for the reporting period.

### Treasury Growth

The change in treasury value attributable to retained capital, realized yield, protocol revenue, market movement, and other approved treasury activity. Treasury growth should be analyzed together with capital inflows and outflows so that new capital formation is not confused with investment performance.

## Reporting framework

A treasury report can include:

| Metric                   | Purpose                                                   |
| ------------------------ | --------------------------------------------------------- |
| Opening Treasury Value   | Starting capital base for the period                      |
| Capital Inflows          | New capital added during the period                       |
| Capital Outflows         | Approved transfers or reductions in treasury capital      |
| Realized Yield           | Yield actually received or realized                       |
| Protocol Revenue         | Revenue generated from protocol activity                  |
| Unrealized P\&L          | Mark-to-market movement in open positions                 |
| Operating Expenses       | Approved expenditure funded from revenue where applicable |
| Buybacks / Burns         | Completed ONMX value-capture activity                     |
| Stablecoin Distributions | Completed eligible distributions where applicable         |
| Closing Treasury Value   | End-of-period treasury value                              |
| Available Liquidity      | Capital immediately or near-term available under policy   |
| Deployed Capital         | Capital allocated to approved productive positions        |

## Performance calculation

Performance reporting distinguishes between **capital formation** and **return on deployed capital**.

A simplified period return can be expressed as:

```
Economic P&L = Closing Treasury Value
             - Opening Treasury Value
             - Net External Capital Inflows
             + Net External Capital Outflows
```

The denominator used for any return percentage depends on the reporting period and the timing of capital flows. Where capital enters or exits during a period, a time-weighted or cash-flow-adjusted methodology can be used to avoid overstating or understating performance.

Any public performance percentage should identify:

* the measurement period,
* the starting and ending dates,
* whether the figure is realized, unrealized, or combined,
* whether fees and expenses are included,
* whether external capital flows are excluded from performance,
* whether the result is annualized.

## Annualization

Annualized figures are presented only when the underlying observation period and methodology are disclosed.

{% hint style="warning" %}
Annualization converts a period result into an annualized rate and does not imply that the observed result will continue for a full year.

Short-period performance can be especially volatile and should not be interpreted as a guaranteed future rate.
{% endhint %}

## Asset valuation

Treasury assets can require different valuation methods.

### Stablecoins

Valued using an approved market or redemption reference, subject to depeg and liquidity considerations.

### Liquid Crypto Assets

Valued using approved market data and a defined reporting timestamp.

### Yield-Bearing Positions

Valued using the redeemable or marked position value where observable, with accrued income separated when needed for reporting clarity.

### Tokenized RWAs

Valuation can incorporate issuer NAV, market price, redemption value, accrued income, settlement status, custody status, and foreign-exchange conversion where applicable.

### Credit Positions

Valuation can incorporate principal outstanding, accrued economic return, payment status, collateral coverage, impairment, default status, recovery assumptions, and secondary-market pricing where available.

## Realized vs. unrealized results

Onchain Matrix separates realized yield from unrealized asset-price movement wherever practical.

This distinction is important because a treasury can show a higher market value without having realized that gain, while realized yield can be received even when the market value of another treasury position declines.

## Treasury reporting and public transparency

Public reporting is designed to provide meaningful accountability without exposing exact future trade timing, transaction-level strategy instructions before execution, sensitive signer details, or other information that could create an avoidable front-running or security risk.

Reporting can include:

* treasury value,
* allocation by approved category,
* available liquidity,
* deployed capital,
* realized yield,
* protocol revenue,
* material policy changes,
* completed buybacks and burns,
* completed eligible stablecoin distributions,
* supply and vesting information,
* relevant onchain verification references.

## Onchain reconciliation

Where practical, official reporting is reconciled against independently reviewable evidence such as:

* treasury wallet balances,
* verified smart-contract positions,
* Gnosis Safe transaction history,
* vesting and lock contracts,
* protocol transaction records,
* third-party custody or RWA records where applicable.

Certain offchain or tokenized-RWA positions can require issuer, custodian, administrator, or settlement records in addition to blockchain data.

## Reporting principle

The objective of treasury reporting is not to maximize the frequency of headline performance claims. It is to provide a consistent record of capital formation, deployment, risk, revenue, and treasury growth that can be evaluated over time.
