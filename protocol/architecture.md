---
description: The modular architecture of Onchain Matrix and the responsibilities of each protocol layer.
---

# Protocol Architecture

Onchain Matrix is designed as a modular capital system. Each layer has a distinct responsibility so that treasury management, credit, security, risk, and token economics do not depend on one monolithic component.

## Architecture layers

### Treasury layer

The treasury layer forms and holds protocol-owned capital. It is responsible for liquidity reserves, allocation policy, strategy exposure, and treasury growth.

### Deployment layer

The deployment layer routes approved capital into permitted assets and strategies. Execution can be constrained by allocation limits, liquidity requirements, risk tiers, and market conditions.

### Credit layer

The credit layer is designed to support:

- P2P matching,
- pool-based liquidity,
- treasury participation,
- collateralized borrowing,
- structured repayment and default terms,
- tokenized debt positions,
- secondary-market liquidity.

### Revenue layer

The revenue layer aggregates treasury yield and protocol fees. Revenue allocation can support operations, reserves, treasury growth, buybacks, burns, eligible distributions, and expansion.

### Risk layer

Financial risk controls govern collateral standards, LTV thresholds, liquidation rules, debt ceilings, strategy exposure, liquidity, and market-response parameters.

### Security layer

Security controls govern custody, administrative permissions, smart-contract deployment, upgrade paths, monitoring, and emergency response.

## Separation of concerns

Financial risk and cybersecurity are intentionally treated separately:

- **Risk management** asks whether capital should be exposed to a position or strategy.
- **Security architecture** asks who can act, how contracts can change, how keys are protected, and how the protocol responds to compromise.

This separation makes the control framework easier to reason about, review, and audit.
