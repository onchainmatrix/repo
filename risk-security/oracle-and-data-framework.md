# Oracle and Data Framework

How Onchain Matrix is designed to source, validate, and use market and protocol data for treasury management, collateralized credit, risk controls, and reporting.

Onchain Matrix depends on external and onchain data for objective execution. Incorrect, stale, manipulated, or illiquid pricing can create material loss even when the surrounding smart contracts operate as designed.

Oracle and data risk are therefore treated as part of the protocol's risk framework rather than as a simple technical integration.

## Where data can be used

Data inputs can support:

* Treasury valuation
* Allocation and rebalancing decisions
* Strategy monitoring
* Collateral valuation
* LTV calculations
* Warning or margin zones
* Liquidation thresholds
* Debt-ceiling and exposure monitoring
* RWA valuation
* Treasury reporting
* Performance measurement
* Circuit breakers and risk-off controls

Not every function requires the same data source or update frequency.

## Data-source principles

Data sources should be evaluated based on the function they serve. Selection criteria can include:

* Reliability
* Market coverage
* Liquidity and market depth of the referenced asset
* Resistance to manipulation
* Update frequency
* Transparency of methodology
* Operational history
* Decentralization where appropriate
* Fallback availability
* Legal or settlement relevance for RWAs
* Compatibility with the relevant network and contract architecture

A widely used data source can still be unsuitable if the underlying market is thin, fragmented, stale, or operationally unreliable.

## Price validation

Where appropriate, protocol logic should be able to reject or restrict data that fails defined validation conditions.

Potential controls can include:

* **Staleness checks** — reject data older than the permitted time window
* **Deviation checks** — flag or restrict an abnormal move from a prior or reference price
* **Cross-source comparison** — compare multiple observations where technically appropriate
* **Market-depth checks** — avoid treating a quoted price as fully executable when liquidity is insufficient
* **Fallback logic** — define what happens when a primary source fails or becomes unreliable
* **Circuit breakers** — restrict activity rather than continue using questionable data

The correct response to bad data is not always to substitute another price automatically. In some conditions, pausing or restricting new exposure can be safer.

## Collateral valuation

Collateralized credit requires more than a displayed market price.

Approved collateral should also be evaluated for:

* Liquidity
* Volatility
* Executable market depth
* Slippage under stressed conditions
* Venue reliability
* Custody and settlement characteristics
* Oracle availability
* Concentration risk
* Legal or issuer structure where relevant

A position can appear overcollateralized and still create losses if the collateral cannot be sold efficiently during a stressed market.

## LTV and liquidation data

For credit positions, price data can influence:

{% stepper %}
{% step %}
## Current collateral value
{% endstep %}

{% step %}
## Current LTV
{% endstep %}

{% step %}
## Warning or margin status
{% endstep %}

{% step %}
## Liquidation eligibility
{% endstep %}

{% step %}
## Recovery value after default
{% endstep %}
{% endstepper %}

The live credit implementation should publish the exact oracle source, calculation conventions, update assumptions, and fallback procedures for each supported collateral type before that collateral is enabled.

## RWA data

Tokenized RWAs can require additional data beyond an onchain market price.

Depending on the instrument, relevant inputs can include:

* Issuer or administrator NAV
* Exchange or market price
* Redemption value
* Accrued income
* Settlement status
* Custody status
* Trading hours
* Stale-price windows
* Currency conversion rates

A tokenized representation does not eliminate issuer, custody, pricing, legal, redemption, or settlement risk.

## Treasury reporting data

Treasury reporting should distinguish between data used for execution and data used for reporting.

A dashboard can display frequent indicative values, while an official period-end treasury report can use a defined valuation timestamp and reconciliation process.

See **Treasury Reporting & Performance Methodology** for reporting definitions.

## Data-provider concentration

Using one provider for every asset can create concentration risk. Where appropriate, the protocol can diversify data dependencies or use independent checks.

The objective is not to maximize the number of providers. It is to ensure that the reliability of a critical protocol function does not depend on an unexamined single source.

## Failure behavior

When data is missing, stale, inconsistent, or materially unreliable, protocol behavior should favor protection over forced continuity.

Depending on the affected function, responses can include:

* Rejecting a transaction
* Pausing new borrowing
* Preventing new deployment
* Reducing exposure
* Switching to an approved fallback
* Requiring manual or multisig review
* Temporarily disabling the affected asset or strategy

## Public documentation

When production oracle infrastructure is selected, the protocol should publish, where appropriate:

* Provider or data-source name
* Supported asset or market
* Feed or contract address
* Network
* Update or heartbeat assumptions
* Staleness policy
* Deviation or validation logic
* Fallback behavior
* Material changes to the data architecture

Provider names should not be treated as final until the applicable production integration is live and verified.

## Oracle risk remains material

No oracle framework can guarantee accurate or executable pricing under every market condition.

Oracle controls are designed to reduce the probability and impact of bad data. They do not remove market, liquidity, smart-contract, issuer, or settlement risk.
