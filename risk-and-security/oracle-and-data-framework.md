# Oracle and Data Framework

Onchain Matrix uses market and protocol data to support treasury management, collateralized credit, risk controls, and reporting. Data quality is treated as a risk-management issue because a correct smart contract can still produce an unsafe outcome when its inputs are stale, manipulated, or economically unreliable.

## Data use across the protocol

Data inputs can support:

* treasury valuation,
* allocation and rebalancing decisions,
* strategy monitoring,
* collateral valuation,
* LTV calculations,
* warning or margin zones,
* liquidation thresholds,
* debt-ceiling and exposure monitoring,
* RWA valuation,
* treasury reporting,
* performance measurement,
* circuit breakers and risk-off controls.

Not every function requires the same source, update frequency, or validation model.

## Data-source principles

Data sources are evaluated according to the function they serve. Relevant criteria include:

* reliability,
* market coverage,
* executable liquidity and market depth,
* resistance to manipulation,
* update frequency,
* transparency of methodology,
* operational history,
* decentralization where appropriate,
* fallback availability,
* legal and settlement relevance for RWAs,
* compatibility with BNB Chain and the relevant contract architecture.

A widely used market price can still be unsuitable when the underlying market is thin, fragmented, stale, or difficult to exit.

## Price validation

Protocol logic can restrict or reject data that fails defined validation conditions.

Potential controls include:

* **Staleness checks** — data older than the permitted window can be rejected.
* **Deviation checks** — abnormal price moves can trigger additional validation or restrictions.
* **Cross-source comparison** — multiple observations can be compared where appropriate.
* **Market-depth checks** — a quoted price is not treated as fully executable when liquidity is insufficient.
* **Fallback logic** — approved behavior is defined for unavailable or unreliable primary sources.
* **Circuit breakers** — protocol activity can be restricted rather than continued with questionable data.

{% hint style="info" %}
The safest response to bad data is not always automatic substitution. In some market conditions, restricting new exposure is preferable to forcing continuity.
{% endhint %}

## Collateral valuation

Collateralized credit requires more than a displayed market price. Approved collateral is also evaluated for:

* liquidity,
* volatility,
* executable market depth,
* stressed-market slippage,
* venue reliability,
* custody and settlement characteristics,
* oracle availability,
* concentration risk,
* legal or issuer structure where relevant.

{% hint style="warning" %}
An overcollateralized position can still generate loss if the collateral cannot be exited efficiently during stress.
{% endhint %}

## LTV and liquidation data

For credit positions, validated market data can influence:

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

Before a collateral type is enabled in a live credit product, the production implementation is expected to expose the applicable data source, valuation convention, update assumptions, and fallback behavior.

## RWA data

Tokenized RWAs can require additional inputs beyond an onchain spot price. Depending on the instrument, relevant data can include:

* issuer or administrator NAV,
* exchange or market price,
* redemption value,
* accrued income,
* settlement status,
* custody status,
* trading hours,
* stale-price windows,
* currency conversion rates.

{% hint style="warning" %}
Tokenization does not eliminate issuer, custody, pricing, legal, redemption, or settlement risk.
{% endhint %}

## Execution data vs. reporting data

Treasury reporting distinguishes between data used for execution and data used for public reporting.

A dashboard can display frequent indicative values, while an official period-end report can use a defined valuation timestamp and reconciliation process. This separation reduces ambiguity between live operational estimates and formal performance reporting.

## Data-provider concentration

Critical protocol functions are not intended to depend on an unexamined single source. Where appropriate, independent checks or diversified data dependencies can reduce provider concentration risk.

The objective is not to maximize the number of providers. It is to make the reliability assumptions of each critical function explicit and testable.

## Failure behavior

When required data is missing, stale, inconsistent, or materially unreliable, protocol behavior is designed to favor protection over forced continuity.

Responses can include:

* rejecting a transaction,
* pausing new borrowing,
* preventing new deployment,
* reducing exposure,
* switching to an approved fallback,
* requiring controlled manual or multisig review,
* temporarily disabling the affected asset or strategy.

{% hint style="warning" %}
No oracle framework can guarantee accurate or executable pricing under every market condition. Oracle controls reduce risk; they do not remove market, liquidity, smart-contract, issuer, or settlement risk.
{% endhint %}
