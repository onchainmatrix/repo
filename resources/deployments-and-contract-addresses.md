# Deployments and Contract Addresses

Onchain Matrix is designed so that important protocol activity can be independently verified onchain.

This page is the canonical registry for production contract addresses, treasury control addresses, Magna vesting and lock infrastructure, and future protocol deployments.

{% hint style="warning" %}
Always verify an address against the official Onchain Matrix website, this documentation, and the relevant block explorer before interacting with it.

Addresses from social posts, direct messages, search results, or unofficial profiles should not be treated as authoritative.
{% endhint %}

## Current production registry

| Component                                          | Network   | Status               | Address                                      | Verification                                    |
| -------------------------------------------------- | --------- | -------------------- | -------------------------------------------- | ----------------------------------------------- |
| ONMX Token                                         | BNB Chain | Live                 | `0x0D60CC169b26be7fCcf0dEcB3B1Ee337fc5cbE5C` | BscScan + official Onchain Matrix channels      |
| Treasury Address                                   | BNB Chain | Published            | `0x92f6fdc4cc90ce24e15c1bca4413f6a7e11af4be` | BscScan + official Onchain Matrix documentation |
| Seed Contract                                      | BNB Chain | Launch-stage         | Not yet published                            | Added when production deployment is activated   |
| Seed Vesting — Magna, powered by Kraken            | BNB Chain | Implementation stage | Not yet published                            | Magna production deployment + BscScan           |
| Treasury Reserve & LP — Magna, powered by Kraken   | BNB Chain | Implementation stage | Not yet published                            | Magna production deployment + BscScan           |
| Team & Advisors Vesting — Magna, powered by Kraken | BNB Chain | Implementation stage | Not yet published                            | Magna production deployment + BscScan           |
| Presale Contract                                   | BNB Chain | Planned              | Not yet published                            | Added at production deployment                  |
| Liquidity Contracts                                | BNB Chain | Planned              | Not yet published                            | DEX deployment + BscScan                        |
| Credit Contracts                                   | BNB Chain | Roadmap              | Not yet deployed                             | Added before production activation              |
| Pool / Marketplace Contracts                       | BNB Chain | Roadmap              | Not yet deployed                             | Added before production activation              |

## Contract status

A production address is listed only after the relevant deployment is intended for public protocol use.

The registry distinguishes between:

* **Live** — deployed and available for current protocol use.
* **Published** — an official address that can be independently verified onchain.
* **Launch-stage / Implementation stage** — production implementation is being prepared but the authoritative address has not yet been published.
* **Planned / Roadmap** — part of the protocol architecture but not yet a production deployment.

Test deployments, development contracts, and internal infrastructure are not official production addresses.

## Magna production infrastructure

Magna, powered by Kraken, has been selected as ONMX token lifecycle infrastructure for material vesting and lock structures.

Once production deployments are active, this registry should identify separately:

### Treasury Reserve & LP

* Allocation: 725,000,000 ONMX / 72.5%
* Structure: 8 years
* Magna production address
* current restricted balance
* relevant BscScan verification

### Team & Advisors

* Allocation: 50,000,000 ONMX / 5%
* Structure: 4-year vesting
* Magna production address or allocation reference where public
* aggregate vested / restricted status where publicly available

### Seed

* Allocation: 25,000,000 ONMX / 2.5%
* Structure: 6-month cliff + 18-month linear vesting
* monthly claim availability after the cliff
* Magna production vesting address
* BscScan verification

{% hint style="info" %}
The production contracts and current onchain state are authoritative for live balances and release mechanics.
{% endhint %}

## Custody and control

Magna supports vesting, claims, custody, and escrow workflows. The exact ONMX custody structure depends on the final production contracts, vaults, wallets, and custody configuration.

{% hint style="warning" %}
Do not infer custody solely from the platform name.
{% endhint %}

When the production configuration is finalized, this registry should identify the relevant controlling address, Safe, vault, custodian, or other control structure where appropriate.

## Upgradeable components

Where a production component is upgradeable, the registry should identify the user-facing proxy, active implementation, controlling authority, and applicable approval or delay path.

{% hint style="warning" %}
A verified proxy address alone does not fully describe upgrade risk.
{% endhint %}

## Treasury and multi-signature verification

Critical treasury authority is structured around multi-party authorization rather than unilateral control by one wallet or key.

Public verification can include:

* controlling Safe address,
* configured approval threshold,
* executed treasury transactions,
* administrative transactions,
* contract ownership transfers,
* timelock activity where applicable.

Personal signer identities, credentials, recovery material, and sensitive security information are not part of the public verification model.

## Source hierarchy

For deployment data, the following order of authority applies:

{% stepper %}
{% step %}
## Live production contracts and current onchain state
{% endstep %}

{% step %}
## Current official Onchain Matrix GitBook
{% endstep %}

{% step %}
## Current official Onchain Matrix website
{% endstep %}

{% step %}
## Current transaction-specific Terms or protocol interface
{% endstep %}

{% step %}
## Archived presentations, Litepapers, announcements, or social posts
{% endstep %}
{% endstepper %}

Historical materials do not override current production contracts or onchain records.
