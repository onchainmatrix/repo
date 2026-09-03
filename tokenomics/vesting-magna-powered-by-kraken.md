# Vesting: Magna Powered by Kraken

## ONMX Token Lifecycle, Vesting & Supply Infrastructure

Onchain Matrix has selected **Magna, powered by Kraken**, as third-party token lifecycle infrastructure for ONMX.

The integration is intended to support critical ONMX supply-management functions through dedicated infrastructure rather than relying only on internal administration. The scope includes allocation management, vesting, locking, stakeholder claims, supply tracking, and the applicable custody or escrow workflows used in the final production configuration.

Magna continues to operate as a standalone token-management platform after its acquisition by Payward in 2026 and is now powered by Kraken.

## Why this matters for Onchain Matrix

Token supply discipline is stronger when it can be independently observed and verified.

For Onchain Matrix, the Magna integration is designed to provide:

* **Independent token lifecycle infrastructure** for restricted ONMX allocations.
* **Long-duration supply discipline** through defined vesting and lock schedules.
* **Stakeholder visibility** into individual allocations, unlocks, vesting progress, and claimable balances.
* **Onchain verification** of production vesting and lock activity.
* **Structured claims infrastructure** so eligible tokens can be claimed when the applicable schedule permits.
* **Operational separation** between Onchain Matrix treasury policy and the infrastructure used to administer restricted token supply.
* **Institutional infrastructure alignment** through Magna's integration into the broader Kraken / Payward platform.

{% hint style="info" %}
The purpose is not to make restricted ONMX liquid earlier. It is to make the applicable release rules clearer, more transparent, and more independently verifiable.
{% endhint %}

## ONMX schedules supported through the token lifecycle framework

Different ONMX allocations follow different release structures.

| Allocation            |                   Supply | Current vesting / lock structure                                                              |
| --------------------- | -----------------------: | --------------------------------------------------------------------------------------------- |
| Treasury Reserve & LP | 725,000,000 ONMX / 72.5% | Long-duration 8-year linear vesting structure through Magna                                   |
| Team & Advisors       |   50,000,000 ONMX / 5.0% | 4-year linear vesting through Magna                                                           |
| Seed                  |   25,000,000 ONMX / 2.5% | 6-month cliff followed by 18-month linear vesting; monthly claim availability after the cliff |
| Other allocations     | As defined in Tokenomics | Governed by their applicable production release terms                                         |

{% hint style="info" %}
The **1,000,000,000 ONMX maximum supply does not itself vest over eight years**. The eight-year structure applies to the **72.5% Treasury Reserve & LP allocation**.&#x20;
{% endhint %}

## Treasury Reserve & LP — 8-year structure

The **725,000,000 ONMX Treasury Reserve & LP allocation** is intended to use Magna for a long-duration eight-year vesting or lock structure.

The purpose of this structure is to support:

* long-term treasury alignment,
* supply discipline,
* independent infrastructure,
* public verification of restricted supply,
* clearer separation between restricted treasury supply and circulating public float.

The production Magna deployment and corresponding onchain records will be authoritative for the live restricted balance, release state, and applicable mechanics.

{% hint style="info" %}
The existence of a vesting or lock schedule does not mean that released tokens will automatically be sold. Treasury deployment and any market activity remain subject to treasury policy, protocol requirements, liquidity, legal considerations, and market conditions.
{% endhint %}

## Team & Advisors — 4-year vesting

The **50,000,000 ONMX Team & Advisors allocation**, representing **5% of maximum supply**, is intended to vest through Magna over **four years**.

This provides long-term alignment between the team, protocol development, and the broader ONMX ecosystem.

The production Magna schedule will determine the authoritative start date, release intervals, vested balance, claimable balance, and completed claims.

## Seed — 6-month cliff + 18-month vesting

The **25,000,000 ONMX Seed allocation**, representing **2.5% of maximum supply**, follows:

* a 6-month cliff,
* followed by 18 months of linear vesting,
* with monthly claim availability after the cliff under the production implementation.

Seed participants will be able to monitor their individual ONMX allocation through the Magna stakeholder dashboard once their allocation has been added and the applicable production infrastructure is active.

## Individual allocation visibility

A Magna stakeholder account is designed to show the stakeholder's **own allocation**.

Depending on the production configuration, the stakeholder can view information such as:

* total ONMX allocated,
* ONMX unlocked to date,
* releasable balance,
* funded balance,
* claimable balance,
* ONMX already received,
* allocation status,
* vesting and unlock timeline,
* receiving wallet,
* claim history.

{% hint style="info" %}
A participant's private Magna account should not be expected to display the individual allocations of other Seed participants, Team members, advisors, or other stakeholders.
{% endhint %}

## Project-level supply transparency

Onchain Matrix will separately maintain public aggregate supply reporting so users, exchanges, and market-data providers can see the overall ONMX structure without exposing private stakeholder information.

The public supply view is intended to distinguish:

* Maximum Supply
* Total Supply
* Circulating Supply
* Treasury-Controlled Supply
* Locked / Vesting Supply
* Treasury Reserve & LP — 8-year schedule
* Team & Advisors — 4-year schedule
* Seed — 6-month cliff + 18-month vesting
* Burned Supply
* Historical releases

Where Magna provides a public project-level dashboard or suitable public verification interface, Onchain Matrix can link it directly from the GitBook and protocol dashboard.

## Custody and control

Magna supports token-management, vesting, claims, custody, and escrow workflows. The exact **ONMX production custody structure** will be determined by the final deployed contracts, vaults, wallets, and custody configuration.

Accordingly, public documentation should describe Magna as the ONMX token lifecycle, vesting, lock, claims, and applicable custody/escrow infrastructure unless and until the final production arrangement establishes a more specific legal or technical custodian role.

The production contracts and controlling addresses remain authoritative.

## Verification

Once production infrastructure is active, Onchain Matrix will publish the relevant verification information in:

**Resources → Deployments & Contract Addresses**

This can include:

* Magna production vesting or lock address,
* covered ONMX allocation,
* applicable schedule,
* current restricted balance,
* historical releases,
* claim transactions,
* BscScan verification,
* relevant controlling wallet or Safe where appropriate.

## Source of truth

For ONMX vesting, locking, claims, and supply status, the order of authority is:

{% stepper %}
{% step %}
## Live production contracts and current onchain state
{% endstep %}

{% step %}
## Production Magna allocation / vesting state
{% endstep %}

{% step %}
## Current official Onchain Matrix GitBook
{% endstep %}

{% step %}
## Current official Onchain Matrix website
{% endstep %}

{% step %}
## Current transaction-specific Terms
{% endstep %}

{% step %}
## Historical presentations, Litepapers, announcements, or social posts
{% endstep %}
{% endstepper %}

Historical materials do not override current production contracts or onchain records.
