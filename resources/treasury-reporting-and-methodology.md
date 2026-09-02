# Treasury Reporting & Methodology

Onchain Matrix is designed around public accountability without publishing operational information that could create unnecessary security, front-running, or market-manipulation risk.

Treasury reporting is intended to make the protocol's capital position and economic activity understandable over time while distinguishing **capital formation**, **treasury performance**, **protocol revenue**, and **market-driven changes in asset value**.

This page defines the reporting principles and metrics that should be used across the Onchain Matrix dashboard, periodic treasury reports, and other official disclosures.

### Reporting Principles

#### Verifiable where possible

Published treasury information should be linked, where practical, to independently reviewable evidence such as:

* onchain wallet balances,
* verified smart contracts,
* multisig activity,
* vesting and lock contracts,
* DeFi position balances,
* transaction history,
* recognized pricing or oracle sources,
* documented RWA valuation sources.

#### Consistent definitions

The same metric should use the same definition across dashboards, reports, presentations, and protocol updates.

If a methodology changes, the change should be disclosed and historical comparisons should be adjusted where reasonably possible.

#### Capital flows are separated from performance

New capital entering the treasury is not investment performance.

Likewise, protocol-directed outflows such as operating expenditures, eligible distributions, or completed buybacks should not automatically be interpreted as investment losses.

Treasury reporting should distinguish:

* external capital inflows,
* treasury investment results,
* protocol revenue,
* protocol-directed outflows,
* changes in asset market value.

#### No pre-announced execution schedule

Transparency does not require publishing exact future trades, strategy instructions, signer identities, or transaction timing before execution.

Onchain Matrix may report executed activity while limiting information that could create front-running, shorting, security, or operational risk.

## Core Treasury Metrics

### Treasury Value

**Treasury Value** represents the estimated fair value of assets and positions economically controlled by the protocol treasury at the reporting timestamp.

It can include:

* stablecoins and liquid reserves,
* approved crypto assets,
* deployed DeFi positions,
* tokenized RWAs,
* approved credit positions,
* liquidity positions,
* accrued but claimable protocol assets where measurable.

Treasury Value should not be calculated from wallet balances alone when capital is deployed into external protocols or other onchain positions.

#### Valuation principle

Each asset should be valued using the most reliable available market or reference price appropriate to that asset.

Where an asset does not have sufficiently reliable price discovery, the report should identify the valuation limitation rather than present false precision.

### Treasury Principal

**Treasury Principal** represents capital contributed to the productive treasury base through approved capital-formation activity.

Principal should be distinguished from:

* generated yield,
* protocol fees,
* unrealized market gains,
* realized trading gains,
* token price movements.

The purpose of this distinction is to show whether treasury growth is being created through additional capital formation, productive deployment, or both.

### Available Liquidity

**Available Liquidity** represents treasury capital that is readily accessible for deployment, reserves, liquidity requirements, or risk response without requiring a material unwind of longer-duration positions.

Available liquidity may include stablecoins and other highly liquid approved assets.

It should not automatically include capital that is:

* locked,
* subject to withdrawal delays,
* committed to credit positions,
* deployed in illiquid strategies,
* restricted by contractual settlement terms.

### Deployed Capital

**Deployed Capital** represents treasury assets actively allocated to approved strategies, positions, or market infrastructure.

This can include:

* yield strategies,
* liquidity positions,
* approved crypto allocation,
* tokenized RWA exposure,
* future approved credit participation.

Deployed Capital should be reported separately from Available Liquidity so users can distinguish productive deployment from immediate reserves.

## Yield & Performance Metrics

### Realized Yield

**Realized Yield** is income or return that has been received, settled, or otherwise economically realized by the treasury during the reporting period.

Examples can include:

* staking or protocol rewards received,
* realized lending or credit income,
* realized strategy yield,
* interest-like or fixed economic returns where applicable,
* realized trading or liquidity income.

Realized Yield excludes new capital contributed to the treasury.

### Unrealized P\&L

**Unrealized Profit or Loss** represents changes in the estimated market value of assets or positions that have not yet been realized through sale, settlement, repayment, or another closing transaction.

Examples include:

* BTC, ETH, BNB, or other approved asset price movements,
* changes in tokenized RWA valuation,
* mark-to-market changes in credit or liquidity positions.

Unrealized P\&L can reverse and should not be presented as realized income.

### Realized P\&L

**Realized Profit or Loss** represents gains or losses that have become economically final through a completed sale, repayment, liquidation, settlement, or other closed transaction.

### Treasury Performance

Treasury performance should measure economic results independently from new capital entering or leaving the treasury.

A simplified reporting framework is:

**Treasury Performance = Change in Treasury Value adjusted for external capital flows and protocol-directed outflows.**

Reports should disclose the specific calculation used whenever a return percentage is published.

Capital raised through Seed, Presale, Public Sale, or other treasury-formation activity should not be counted as investment return.

### Cumulative Performance

**Cumulative Performance** represents the compounded performance of the treasury from a clearly identified starting date.

Every published cumulative figure should state:

* the measurement start date,
* the measurement end date or snapshot time,
* whether the result is gross or net,
* whether protocol-directed outflows are adjusted for,
* the principal methodology used.

Cumulative performance should not be calculated simply by comparing treasury size at two dates when additional capital entered the treasury during the period.

### Annualized Return

Where an annualized figure is presented, the calculation should be based on the measured return over the stated period and clearly identified as annualized.

Annualization is a mathematical normalization of historical results. It is not a forecast or guarantee that the same rate will continue.

Very short measurement periods should not be presented in a way that creates a misleading impression of expected annual performance.

## Protocol Revenue Metrics

### Gross Protocol Revenue

**Gross Protocol Revenue** represents revenue generated by protocol activity before protocol operating expenditures and other approved uses.

Potential revenue sources can include:

* treasury yield,
* credit spread participation,
* origination fees,
* servicing fees,
* pool activity,
* marketplace or secondary-market activity,
* other protocol services as they become active.

Capital raised for treasury formation is not Protocol Revenue.

### Revenue After Operations

**Revenue After Operations** represents Gross Protocol Revenue less approved operating expenditures attributable to the reporting period.

The metric is intended to show how much protocol-generated revenue remains available for treasury growth, reserves, value-capture mechanisms, or other approved uses.

### Operating Budget Ratio

Where reported, the **Operating Budget Ratio** measures operating expenditures relative to Gross Protocol Revenue for the same period.

**Operating Budget Ratio = Operating Expenditures ÷ Gross Protocol Revenue**

A lower ratio can indicate improving operating leverage, but it should not be interpreted in isolation from security, development, liquidity, and infrastructure requirements.

### Revenue Coverage Ratio

Where reported, the **Revenue Coverage Ratio** measures how many times Gross Protocol Revenue covers approved operating expenditures.

**Revenue Coverage Ratio = Gross Protocol Revenue ÷ Operating Expenditures**

A value above 1.0x indicates that reported protocol revenue exceeded reported operating expenditures for the period.

## Allocation Reporting

Treasury allocation should be reported using current estimated fair values rather than original purchase cost unless otherwise stated.

Allocation categories can include:

* Stablecoin & Liquidity Base
* Core Crypto Allocation
* Base Yield Strategies
* RWAs & Approved Credit
* Selective Higher-Yield Opportunities
* Other Approved Positions

Each report should state the snapshot date and whether percentages are based on gross treasury value or another defined denominator.

Onchain Matrix does not commit to permanently fixed allocation weights. Treasury allocation can change in response to risk, liquidity, market conditions, strategy quality, protocol requirements, and treasury policy.

## Pricing & Valuation Sources

### Liquid crypto assets

Liquid crypto assets should use transparent market or oracle data from recognized sources appropriate to the asset and reporting context.

Where appropriate, reporting can use a time-weighted or consolidated reference rather than a single isolated trade.

### Stablecoins

Stablecoins should be valued using observable market value when a material deviation from their intended peg exists.

A stablecoin should not automatically be assumed to equal one U.S. dollar during a depeg or impairment event.

### DeFi positions

DeFi positions should be valued using the underlying redeemable or claimable asset value where it can be determined reliably.

Material exit fees, lock periods, withdrawal restrictions, or impaired liquidity should be disclosed where relevant.

### Tokenized RWAs

Tokenized RWA positions should use the most appropriate available issuer, administrator, market, oracle, or independently verifiable valuation source.

Reporting should identify material differences between onchain token price, reference asset value, and redemption value where relevant.

### Credit positions

Credit positions should not automatically be valued at face value when repayment risk, collateral impairment, default, or liquidity conditions materially affect economic value.

## Reporting Frequency & Snapshot Time

Each dashboard or treasury report should clearly state:

* the reporting period,
* the snapshot timestamp,
* the pricing timestamp or methodology,
* the data sources used,
* whether figures are preliminary or final.

Dashboard values may update more frequently than formal treasury reports.

A displayed value should not imply real-time liquidity when an underlying position has settlement, lock, or withdrawal constraints.

## Buybacks, Burns & Distributions

Treasury reporting should separately identify completed:

* ONMX buybacks,
* ONMX burns,
* eligible stablecoin distributions or airdrops,
* operating expenditures,
* treasury transfers.

Buybacks and distributions are not guaranteed and remain subject to protocol policy, treasury conditions, market liquidity, legal requirements, and operational readiness.

Where a buyback is completed, reporting should identify the amount of treasury capital used and the resulting ONMX treatment.

Where ONMX is burned, the corresponding onchain burn transaction should be publicly verifiable.

## Reporting Integrity

Onchain Matrix should avoid presenting:

* capital raised as investment return,
* unrealized gains as realized yield,
* gross yield as net protocol revenue,
* fixed-value assumptions during material market dislocations,
* projected results as realized performance,
* roadmap revenue as current revenue.

Historical results, treasury models, and return scenarios do not guarantee future performance.

The objective of treasury reporting is not to maximize headline numbers. It is to provide a consistent, understandable, and verifiable record of how protocol capital is formed, deployed, preserved, and grown.
