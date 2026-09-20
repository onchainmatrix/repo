# Supply, Allocation & Vesting

ONMX has a fixed maximum supply of **1,000,000,000 tokens** on BNB Chain.

The supply structure is designed to distinguish between maximum supply, restricted supply, treasury-controlled supply, vesting supply, and tokens reasonably available for public circulation.

## Allocation

| Category                   | % of Supply |            Tokens |
| -------------------------- | ----------: | ----------------: |
| Treasury Reserve & LP      |       72.5% |       725,000,000 |
| Public Sale                |       10.0% |       100,000,000 |
| Team & Advisors            |        5.0% |        50,000,000 |
| Seed                       |        2.5% |        25,000,000 |
| Presale                    |        2.5% |        25,000,000 |
| Community Participation    |        2.5% |        25,000,000 |
| Ecosystem Growth           |        2.5% |        25,000,000 |
| Infrastructure Development |        2.5% |        25,000,000 |
| **Total**                  |    **100%** | **1,000,000,000** |

## Core Treasury Allocation — 87.5%

The protocol identifies **87.5% of maximum ONMX supply** as the Core Treasury Allocation:

**72.5% Treasury Reserve & LP + 10.0% Public Sale + 2.5% Presale + 2.5% Seed = 87.5%.**

This classification reflects the intended role of these allocations in treasury formation and launch capital flows.

{% hint style="info" %}
It does **not** mean that 87.5% of ONMX is immediately circulating, unlocked, available for sale, or simultaneously deployed.
{% endhint %}

## Magna, powered by Kraken

Onchain Matrix has selected **Magna, powered by Kraken**, as third-party token lifecycle infrastructure for ONMX vesting, locking, allocation management, stakeholder claims, supply tracking, and the applicable custody or escrow workflows used in the final production configuration.

The purpose is to place material restricted ONMX allocations under defined, independently verifiable lifecycle infrastructure rather than relying only on discretionary internal administration.

Production Magna contracts, vaults, wallets, and onchain records will be authoritative for the live restricted balance, vesting status, and claimable supply.

See:

**Tokenomics → Magna, powered by Kraken**

## Treasury Reserve & LP — 72.5%

The **725,000,000 ONMX Treasury Reserve & LP allocation** is intended to use a long-duration **eight-year** structure through Magna.

The reserve structure is designed to provide:

* Long-duration supply discipline
* Independent lifecycle infrastructure
* Public onchain verification
* Separation between restricted treasury supply and public circulating supply
* An auditable history of releases

{% hint style="info" %}
The eight-year structure does not imply a mechanical eight-year market-sale schedule.

Released or eligible ONMX is not automatically sold. Treasury deployment and market activity remain subject to treasury policy, protocol needs, liquidity, legal considerations, and market conditions.
{% endhint %}

## Team & Advisors — 5%

The **50,000,000 ONMX Team & Advisors allocation** is intended to vest through Magna over **four years**.

This structure is designed to support long-term alignment between the team, advisors, protocol development, and the ONMX ecosystem.

The production Magna allocation will determine the authoritative start date, vesting state, claimable balance, and completed releases.

## Seed — 2.5%

The **25,000,000 ONMX Seed allocation** is structured with:

* A **6-month cliff**
* Followed by **18 months of linear vesting**
* **Monthly claim availability after the cliff** under the production implementation

Seed participants will be able to monitor their own allocations and claim status through the Magna stakeholder dashboard once production onboarding is active.

See:

**Seed Access → Magna Dashboard — Vesting & Claims**

## Full-supply visibility

The full **1,000,000,000 ONMX maximum supply** should be displayed in public supply reporting together with the status of each allocation.

The eight-year vesting or lock structure applies specifically to the **72.5% Treasury Reserve & LP allocation**, not automatically to every ONMX token.

Public reporting should separately identify:

* Maximum Supply
* Total Supply
* Circulating Supply
* Locked / Vesting Supply
* Treasury-Controlled Supply
* Team & Advisor Vesting
* Seed Vesting
* Burned Supply

## Other allocations

Final release, custody, transfer, lock, or vesting rules for other allocations are governed by the applicable production contracts, protocol documentation, transaction-specific Terms, and current onchain records.

{% hint style="info" %}
An allocation's economic purpose is not the same as its circulating status.
{% endhint %}

## Verification

Once activated, relevant Magna production addresses and ONMX release infrastructure will be listed under:

**Resources → Deployments & Contract Addresses**

Users and market-data providers should use the production contracts and current onchain state rather than historical presentation materials to determine current supply status.
