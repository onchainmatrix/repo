---
description: Custody, access, contract, upgrade, monitoring, and incident-response controls for Onchain Matrix.
---

# Security Architecture

Security is designed across custody, contracts, infrastructure, access control, monitoring, and incident response.

## Multi-signature treasury custody

Critical treasury authority is designed around multi-party approval rather than unilateral control by one wallet or key. Multi-signature custody reduces single-key compromise risk and creates an auditable approval path for sensitive actions.

## Privileged access & key security

Administrative access should be:

- permissioned,
- segmented by role,
- protected by hardened authentication,
- minimized to the access required,
- reviewed as responsibilities change.

Operational processes should avoid unnecessary exposure of signer identities, credentials, recovery material, or sensitive internal infrastructure.

## Smart-contract security

Core contracts should follow disciplined development, testing, verification, review, and deployment procedures. Public contract verification helps users and reviewers confirm deployed bytecode and interfaces.

External security audits should be published when completed. Until an audit is complete and published, documentation should not imply that a contract has been externally audited.

## Timelocked & controlled upgrades

High-impact changes can use defined approval paths and delay periods rather than immediate unilateral execution. Upgrade authority should be constrained, observable, and reduced or disabled when the protocol reaches the appropriate maturity stage.

## Continuous monitoring

Monitoring can cover:

- contract events,
- privileged actions,
- treasury movements,
- infrastructure alerts,
- abnormal behavior,
- oracle issues,
- unexpected changes in protocol state.

## Emergency response

Where technically appropriate, pause modules, restricted new activity, or other incident-response procedures can limit damage during a live event.

Emergency authority itself is sensitive and should be governed by the same custody and access-control principles as other privileged actions.

## Public verifiability

Security claims should be supported by verifiable evidence wherever possible: deployed contracts, multisig transactions, published audit reports, onchain events, and documented control procedures.
