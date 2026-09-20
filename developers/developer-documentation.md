# Developer Documentation

Onchain Matrix is being deployed in phases.

Developer documentation should distinguish between **currently published infrastructure** and **roadmap components** so integrations do not rely on interfaces that have not yet been launched or verified.

### Network

**Primary network:** BNB Chain

**ONMX standard:** BEP-20

**Maximum supply:** 1,000,000,000 ONMX

### Current Public ONMX Contract

`0x0D60CC169b26be7fCcf0dEcB3B1Ee337fc5cbE5C`

Developers should verify the address against the official Onchain Matrix deployment registry and the relevant block explorer before using it in production.

{% hint style="warning" %}
Do not hard-code an address sourced only from a social post, direct message, search-engine result, or third-party token list.
{% endhint %}

## Integration Status

### Current / Launch-Stage Infrastructure

The current public documentation is centered on:

* ONMX token infrastructure,
* treasury formation,
* Seed and launch-stage infrastructure,
* multi-signature treasury controls,
* initial treasury deployment,
* public verification and reporting.

Only interfaces that are publicly deployed and listed in the official deployment registry should be treated as production integrations.

### Roadmap Interfaces

The following remain roadmap components unless and until official deployments are published:

* pool-based collateralized lending,
* P2P structured credit,
* borrower interfaces,
* tokenized debt issuance,
* secondary-market debt liquidity,
* broader tokenized RWA credit integrations,
* expanded credit-market fee and servicing infrastructure.

{% hint style="warning" %}
Do not infer final contract interfaces from roadmap descriptions.
{% endhint %}

## Protocol Architecture

At a high level, Onchain Matrix is organized into the following functional layers.

### Treasury Layer

Responsible for protocol-owned capital, liquidity reserves, allocation policy, strategy exposure, and treasury growth.

### Deployment Layer

Routes approved treasury capital into permitted assets and strategies under allocation, liquidity, and risk controls.

### Credit Layer

Designed to support future:

* P2P matching,
* pool-based liquidity,
* treasury participation,
* collateralized borrowing,
* structured repayment and default terms,
* tokenized debt positions,
* secondary-market liquidity.

### Revenue Layer

Aggregates treasury yield and protocol fees for allocation among approved protocol uses.

### Risk Layer

Defines collateral, LTV, liquidation, debt ceiling, exposure, liquidity, and market-response controls.

### Security Layer

Governs custody, administrative permissions, contract deployment, upgrade paths, monitoring, and emergency response.

## Deployment Registry

The canonical deployment registry should be maintained in:

**Resources → Contracts, Transparency & Public Verification**

The registry can include:

* ONMX token,
* Seed or token-sale contracts,
* vesting contracts,
* treasury reserve lock contracts,
* treasury or multisig addresses,
* future credit contracts,
* future lending pools,
* future marketplace or tokenized-debt contracts.

{% hint style="warning" %}
A contract should not be treated as official until it is published through official Onchain Matrix documentation.
{% endhint %}

## Magna vesting and lock integration

ONMX production vesting and lock deployments are intended to use Magna, powered by Kraken, for material restricted allocations. Developers should treat the official Magna production contracts and current onchain state as authoritative for vesting, restricted balance, claimable balance, and completed claim events. Do not infer a release schedule solely from offchain dates.



* Treasury Reserve & LP — 72.5% — 8-year structure
* Team & Advisors — 5% — 4-year vesting
* Seed — 2.5% — 6-month cliff + 18-month linear vesting

Individual Magna stakeholder accounts are private allocation views. Project-wide circulating-supply analytics should use the official ONMX Supply & Circulating-Supply Transparency methodology.

## Contract Verification

Before integrating an Onchain Matrix contract:

{% stepper %}
{% step %}
### Obtain the address

Obtain the address from the official deployment registry.
{% endstep %}

{% step %}
### Confirm the network

Confirm the network.
{% endstep %}

{% step %}
### Verify the contract

Verify the contract on the relevant block explorer.
{% endstep %}

{% step %}
### Review the source or interface

Review the verified source or interface where available.
{% endstep %}

{% step %}
### Confirm deployment status

Confirm whether the deployment is current, deprecated, paused, or superseded.
{% endstep %}

{% step %}
### Review security information

Review any published security or audit information relevant to that deployment.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
A familiar contract name is not sufficient proof of authenticity.
{% endhint %}

## ABI & Interface Publication

Official ABIs and contract interfaces should be published alongside production deployments when stable.

{% hint style="warning" %}
Until an ABI is officially published or obtainable from a verified deployment, developers should not rely on undocumented methods, reverse-engineered interfaces, or assumptions based on roadmap descriptions.
{% endhint %}

Where a contract is upgradeable or otherwise subject to controlled change, the deployment registry should identify the relevant implementation and control structure when appropriate.

## Onchain Data Integration

### Token Data

Applications integrating ONMX should distinguish:

* maximum supply,
* economically released supply,
* locked supply,
* treasury-controlled supply,
* circulating supply,
* burned supply.

{% hint style="info" %}
`totalSupply()` or a token balance alone should not be treated as a complete circulating-supply methodology.
{% endhint %}

### Treasury Data

Treasury value should not be inferred from a single wallet balance.

Protocol capital can be:

* held as liquid assets,
* deployed into strategies,
* represented by LP or receipt tokens,
* allocated to tokenized RWAs,
* committed to future credit positions.

Applications presenting treasury analytics should use the official Treasury Reporting & Methodology definitions.

### Vesting Data

Where vesting contracts are deployed, interfaces should read the applicable onchain schedule rather than infer unlocks solely from offchain dates.

### Transaction History

Treasury and protocol reporting can reference:

* multisig transactions,
* token transfers,
* contract events,
* vesting events,
* buybacks,
* burns,
* distributions,
* strategy interactions.

Event interpretation should follow the relevant contract version.

## Pricing & Oracle Data

Treasury and future credit integrations can require reliable market data for:

* treasury valuation,
* collateral valuation,
* LTV,
* liquidation thresholds,
* risk monitoring,
* tokenized RWA pricing.

Final oracle providers, fallback rules, staleness thresholds, and deviation controls should be documented with the relevant live contracts.

{% hint style="warning" %}
Developers should not assume that one pricing source applies to every supported asset.
{% endhint %}

## Future Credit Integration

The planned credit lifecycle is:

**Terms & Eligibility → Collateral Lock → Funding → Active Monitoring → Tokenized Debt Position → Hold to Maturity or Approved Secondary Liquidity → Repayment / Resolution**

Future credit interfaces can expose data such as:

* principal,
* collateral,
* maturity,
* LTV,
* warning thresholds,
* liquidation thresholds,
* debt ceilings,
* repayment status,
* default status,
* position ownership,
* tokenized debt metadata.

{% hint style="info" %}
These fields are architectural expectations, not a final ABI specification.

The deployed contracts and official interface documentation will control the final implementation.
{% endhint %}

## Security Considerations for Integrators

Developers should:

* verify every contract address,
* validate the connected network,
* avoid unlimited token approvals where unnecessary,
* surface spender addresses clearly,
* protect signing workflows from domain substitution,
* distinguish read operations from transaction requests,
* validate oracle freshness where relevant,
* handle paused or restricted protocol states,
* avoid assuming that a successful transaction guarantees economic finality in a multi-step workflow.

{% hint style="danger" %}
Applications should never request a user's private key or recovery phrase.
{% endhint %}

## Upgrade & Version Awareness

Onchain Matrix is designed around controlled protocol changes rather than ad hoc execution.

Integrations should be designed to tolerate versioned contracts and interface changes.

Where applicable, official documentation should identify:

* deployment version,
* contract status,
* implementation address,
* controlling multisig or role,
* timelock or delay mechanism,
* migration guidance,
* deprecation status.

Developers should monitor the official changelog and deployment registry before production releases.

## APIs, SDKs & Indexing

{% hint style="warning" %}
No API or SDK should be treated as official unless it is published through the Onchain Matrix documentation or official repositories.
{% endhint %}

Until dedicated developer services are published, verified onchain contracts remain the primary source for protocol state.

Future developer infrastructure can include:

* indexed treasury data,
* protocol analytics endpoints,
* contract SDKs,
* credit-position data,
* tokenized-debt metadata,
* event indexing,
* integration examples.

## Reporting Integration

Applications displaying Onchain Matrix financial data should clearly distinguish:

* Treasury Value,
* Treasury Principal,
* Available Liquidity,
* Deployed Capital,
* Realized Yield,
* Unrealized P\&L,
* Protocol Revenue,
* Operating Expenditures,
* Revenue After Operations.

{% hint style="warning" %}
Capital contributed through Seed, Presale, Public Sale, or other treasury-formation activity should not be displayed as investment return.
{% endhint %}

## Responsible Integration

Production applications should prefer correctness and verification over convenience.

{% hint style="warning" %}
If a contract, interface, address, parameter, or status is not documented through an official Onchain Matrix source, treat it as unverified.
{% endhint %}

For integration questions, use the official contact information published through onchainmatrix.com.
