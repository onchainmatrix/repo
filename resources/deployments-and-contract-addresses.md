# Deployments and Contract Addresses

A canonical registry of Onchain Matrix contracts, treasury addresses, lock and vesting infrastructure, and future protocol deployments.

Onchain Matrix is designed so that important protocol activity can be independently verified onchain wherever practical. This page should be treated as the primary documentation registry for official deployment addresses.

{% hint style="warning" %}
**Verification rule:** Never rely on a contract address copied from an unofficial website, social post, direct message, search result, or third-party profile. Verify addresses against the official Onchain Matrix website, this documentation, and the relevant block explorer before interacting.
{% endhint %}

## Current published addresses

| Component                       | Network   | Status               | Address                                      | Verification                                              |
| ------------------------------- | --------- | -------------------- | -------------------------------------------- | --------------------------------------------------------- |
| ONMX Token                      | BNB Chain | Live / published     | `0x0D60CC169b26be7fCcf0dEcB3B1Ee337fc5cbE5C` | Verify on BscScan and the official Onchain Matrix website |
| Treasury Address                | BNB Chain | Published            | `0x92f6fdc4cc90ce24e15c1bca4413f6a7e11af4be` | Verify on BscScan and official documentation              |
| Seed Contract                   | BNB Chain | Publish when live    | —                                            | Official GitBook + BscScan                                |
| Seed Vesting Contract           | BNB Chain | Publish when live    | —                                            | Official GitBook + vesting provider + BscScan             |
| Treasury Reserve Lock / Vesting | BNB Chain | Implementation stage | —                                            | Official GitBook + third-party lock provider + BscScan    |
| Presale Contract                | BNB Chain | Publish when live    | —                                            | Official GitBook + BscScan                                |
| Liquidity Contracts             | BNB Chain | Publish when live    | —                                            | Official GitBook + DEX + BscScan                          |
| Credit Contracts                | BNB Chain | Roadmap              | —                                            | Official GitBook + BscScan                                |
| Pool / Marketplace Contracts    | BNB Chain | Roadmap              | —                                            | Official GitBook + BscScan                                |

{% hint style="info" %}
Addresses not yet published above should not be inferred from test deployments or unofficial sources.
{% endhint %}



## Upgradeable contracts

Where a contract is upgradeable, the documentation should distinguish between the user-facing proxy and the active implementation.

A verified proxy address alone does not explain who can change the implementation. For upgradeable components, the public registry should therefore identify the controlling authority and any applicable approval or delay process.

High-impact changes are intended to follow controlled approval paths rather than immediate unilateral execution. Upgrade authority should remain observable and can be reduced or disabled as the protocol reaches the appropriate maturity stage.

## Treasury and multisig verification

Treasury custody is designed around multi-party authorization rather than unilateral control by one wallet or key.

The official deployment registry should identify the treasury or multisig address used for critical authority without publishing personal signer identities or sensitive security information.

Public verification can include:

* The multisig address
* Transaction history
* Approval threshold where publicly configured
* Executed treasury actions
* Administrative transactions
* Contract ownership transfers
* Timelock transactions where applicable

## Vesting and lock infrastructure

Token allocations that are subject to vesting or long-duration restrictions should be linked to independently verifiable infrastructure once implemented.

For each vesting or lock arrangement, publish:

* Allocation covered
* Token amount
* Vesting or lock provider
* Relevant contract or vault address
* Start condition or effective date
* Cliff or vesting terms where applicable
* Claim or release mechanics
* Public verification link

The Treasury Reserve & LP allocation is intended to use a long-duration third-party structure over an eight-year period. Magna has been selected as the intended infrastructure provider; final contract addresses and implementation details should be published here only after the production setup is live and verifiable.

## Source hierarchy

If information conflicts across channels, use the following order of authority for deployment data:

1. Live production contracts and onchain state
2. Current official Onchain Matrix GitBook
3. Current official Onchain Matrix website
4. Current transaction-specific Terms or interface
5. Archived presentations, Litepapers, announcements, or social posts

{% hint style="info" %}
Historical documents may describe an earlier deployment state and should not override current onchain records.
{% endhint %}

