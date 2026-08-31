# Deployments and Contract Addresses

Onchain Matrix is designed so that important protocol activity can be independently verified onchain. This page is the canonical registry for production contract addresses, treasury control addresses, vesting and lock infrastructure, and future protocol deployments.

## Verification standard

{% hint style="warning" %}
Always verify an address against the official Onchain Matrix website, this documentation, and the relevant block explorer before interacting with it. Addresses from social posts, direct messages, search results, or unofficial profiles should not be treated as authoritative.
{% endhint %}

## Current production registry

| Component                       | Network   | Status               | Address                                      | Verification                                                   |
| ------------------------------- | --------- | -------------------- | -------------------------------------------- | -------------------------------------------------------------- |
| ONMX Token                      | BNB Chain | Live                 | `0x0D60CC169b26be7fCcf0dEcB3B1Ee337fc5cbE5C` | BscScan + official Onchain Matrix channels                     |
| Treasury Address                | BNB Chain | Published            | `0x92f6fdc4cc90ce24e15c1bca4413f6a7e11af4be` | BscScan + official Onchain Matrix documentation                |
| Seed Contract                   | BNB Chain | Launch-stage         | Not yet published                            | Added to this registry when production deployment is activated |
| Seed Vesting                    | BNB Chain | Launch-stage         | Not yet published                            | Production vesting contract + BscScan                          |
| Treasury Reserve Lock / Vesting | BNB Chain | Implementation stage | Not yet published                            | Magna production deployment + BscScan                          |
| Presale Contract                | BNB Chain | Planned              | Not yet published                            | Added at production deployment                                 |
| Liquidity Contracts             | BNB Chain | Planned              | Not yet published                            | DEX deployment + BscScan                                       |
| Credit Contracts                | BNB Chain | Roadmap              | Not yet deployed                             | Added before production activation                             |
| Pool / Marketplace Contracts    | BNB Chain | Roadmap              | Not yet deployed                             | Added before production activation                             |

## Contract status

A production address is listed only after the relevant deployment is intended for public protocol use. Test deployments, development contracts, and internal infrastructure are not official production addresses.

The registry distinguishes between:

* **Live** — deployed and available for current protocol use.
* **Published** — an official address that can be independently verified onchain.
* **Launch-stage** — implementation is being prepared for production use.
* **Planned / Roadmap** — part of the protocol architecture but not yet a production deployment.

## Upgradeable components

Where a production component is upgradeable, the registry identifies the user-facing proxy, active implementation, controlling authority, and applicable approval or delay process.

A verified proxy address alone does not fully describe upgrade risk. The relevant control path matters because it determines who can change the implementation and under what conditions.

High-impact changes are designed to follow controlled approval paths rather than unilateral execution. Upgrade authority is intended to remain observable and can be reduced, constrained, or disabled as the protocol reaches the appropriate maturity stage.

## Treasury and multi-signature verification

Critical treasury authority is structured around multi-party authorization rather than unilateral control by a single wallet or key. Treasury control uses a Gnosis Safe multi-signature structure.

Public verification can include:

* the controlling Safe address,
* configured approval threshold,
* executed treasury transactions,
* administrative transactions,
* contract ownership transfers,
* timelock activity where applicable.

Personal signer identities, credentials, recovery material, and sensitive security information are not part of the public verification model.

## Vesting and lock infrastructure

Token allocations subject to vesting or long-duration restrictions are intended to use independently verifiable infrastructure.

The **72.5% Treasury Reserve & LP allocation** is intended to use a long-duration third-party structure over an **eight-year period**. **Magna** has been selected as the infrastructure provider for this reserve structure. The production contract or vault address will become part of this registry once the deployment is live and independently verifiable.

The **Seed allocation** is structured with a **6-month cliff followed by 18 months of linear vesting**, with monthly claim availability after the cliff. The production vesting deployment is the authoritative source for claim and release mechanics.

## Source hierarchy

For deployment data, the following order of authority applies:

{% stepper %}
{% step %}
### Live production contracts and current onchain state
{% endstep %}

{% step %}
### Current official Onchain Matrix GitBook
{% endstep %}

{% step %}
### Current official Onchain Matrix website
{% endstep %}

{% step %}
### Current transaction-specific Terms or protocol interface
{% endstep %}

{% step %}
### Archived presentations, Litepapers, announcements, or social posts

Historical materials may describe an earlier deployment state and do not override current production contracts or onchain records.
{% endstep %}
{% endstepper %}
