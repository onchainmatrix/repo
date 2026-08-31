# Smart Contract Architecture

Onchain Matrix is designed as a modular onchain capital system rather than a single monolithic contract. Treasury custody, token supply, capital deployment, vesting, future credit markets, market data, and administrative controls are separated so that each component can have a clearly defined responsibility and permission boundary.

## Architecture overview

```mermaid
%%{init: {"flowchart": {"nodeSpacing": 18, "rankSpacing": 24, "curve": "basis"}, "themeVariables": {"fontSize": "13px"}}}%%
flowchart TB
    A[ONMX Token] --> B[Capital Formation / Sale Infrastructure]
    B --> C[Protocol-Owned Treasury]
    C --> D[Treasury Execution Layer]
    D --> E[Approved Strategies & Assets]
    D --> F[Future Credit Layer]
    F --> G[Collateral & Position Accounting]
    G --> H[Tokenized Debt]
    H --> I[Approved Secondary-Market Infrastructure]
    J[Oracle & Data Layer] --> D
    J --> F
    K[Multi-Sig / Administrative Controls] --> C
    K --> D
    K --> F
    L[Vesting & Lock Infrastructure] --> A
```

The exact production contracts associated with each layer are listed in **Deployments & Contract Addresses** as they become active.

## ONMX token layer

ONMX is deployed on BNB Chain as a BEP-20 ecosystem token with a fixed total supply of 1,000,000,000 ONMX.

The token layer provides the base supply and transfer functionality used by the broader protocol. Token economics are designed around fixed supply, treasury formation, protocol utility, and non-inflationary value capture rather than ongoing minting for rewards.

## Capital-formation layer

Sale and participation infrastructure is designed to control how approved ONMX allocations are released into the ecosystem during seed, presale, public-sale, or other authorized capital-formation activity.

Capital-formation contracts and interfaces can enforce transaction-specific conditions such as:

* allocation limits,
* payment requirements,
* wallet eligibility,
* network requirements,
* vesting or claim rules,
* applicable participation terms.

Production sale contracts are independently listed in the deployment registry.

## Treasury custody layer

Protocol-owned treasury capital is controlled through a Gnosis Safe multi-signature structure rather than a single private key.

The treasury custody layer is responsible for high-impact asset authority. It is intentionally separated from routine automation so that execution systems do not automatically receive unrestricted custody powers.

## Treasury execution layer

The treasury execution layer is designed to route approved capital into permitted assets and strategies under treasury policy.

Execution can be constrained by:

* allocation limits,
* reserve requirements,
* supported asset lists,
* strategy allowlists,
* liquidity requirements,
* risk tiers,
* market conditions,
* emergency restrictions.

As treasury automation matures, routine actions can become more programmatic while policy and high-impact authority remain separately controlled.

## Vesting and lock layer

Vesting and lock infrastructure separates long-duration or restricted supply from normal circulating supply.

The reserve structure is intended to use Magna over an eight-year period for the 72.5% Treasury Reserve & LP allocation. Seed tokens follow a 6-month cliff plus 18-month linear vesting structure.

Production vesting and lock contracts are authoritative for the live balance, unlock state, and claim mechanics.

## Credit layer

The future credit layer is designed as a separate set of contracts and modules supporting:

* P2P structured credit,
* pool-based liquidity,
* treasury participation,
* collateral lock,
* position accounting,
* LTV monitoring,
* repayment,
* liquidation,
* default resolution,
* tokenized debt representation.

Credit-market contracts are roadmap infrastructure until publicly deployed and verified.

## Oracle and data layer

Oracle and data infrastructure supplies or validates the external information used for valuation, collateral health, risk limits, and reporting.

Data authority is separated from asset custody. A data provider does not receive treasury transfer authority simply because its data is used by protocol logic.

## Administrative and emergency controls

Privileged functions are designed around explicit roles and permission boundaries.

Depending on the production component, controls can include:

* multi-signature approval,
* role-based administration,
* timelocked execution,
* pause or restriction modules,
* controlled upgrade authority,
* post-deployment monitoring.

## Proxy and implementation transparency

For upgradeable production components, public documentation distinguishes the proxy address from the active implementation and identifies the applicable control path.

This makes it possible to evaluate not only the code currently serving users but also the authority capable of changing that code.

## Modularity principle

The architecture is designed so that changes to one subsystem do not automatically require unrestricted access to every other subsystem. Treasury custody, risk administration, oracle data, credit operations, and token supply are treated as separate control domains.
