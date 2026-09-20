# ONMX Supply Transparency

## ONMX Supply & Circulating-Supply Transparency

ONMX has a fixed maximum supply of **1,000,000,000 ONMX** on BNB Chain.

Supply transparency distinguishes between maximum supply, current total supply, restricted or vesting supply, treasury-controlled supply, burned supply, and tokens reasonably available for normal public market circulation.

An allocation's economic purpose is not the same as its circulating status.

### Token allocation

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

### Core Treasury Allocation — 87.5%

The Core Treasury Allocation combines:

**72.5% Treasury Reserve & LP + 10.0% Public Sale + 2.5% Presale + 2.5% Seed = 87.5%.**

This classification describes economic purpose. It does not mean that 87.5% is immediately circulating, unlocked, or available for sale.

## Supply categories

### Maximum Supply

The maximum number of ONMX that can exist under the fixed-supply design.

**Maximum Supply: 1,000,000,000 ONMX**

### Total Supply

The amount of ONMX existing onchain after accounting for any permanent supply reductions recognized by the token contract and applicable reporting methodology.

### Circulating Supply

ONMX that is issued and reasonably available for normal public market circulation.

Tokens that remain locked, unvested, unreleased, or otherwise restricted from normal public float are reported separately under the applicable methodology.

Market-data platforms can apply their own circulating-supply methodologies.

### Locked / Vesting Supply

ONMX subject to contractual lock, cliff, linear vesting, or other transfer restrictions that prevent normal public circulation.

### Treasury-Controlled Supply

ONMX held or controlled for treasury, liquidity, ecosystem, infrastructure, or other protocol purposes.

Treasury-controlled supply is not automatically equivalent to public circulating supply.

### Burned Supply

ONMX permanently removed from usable supply through the applicable burn mechanism and recognized by the relevant onchain and reporting methodology.

## Magna, powered by Kraken

Onchain Matrix has selected **Magna, powered by Kraken**, as token lifecycle infrastructure for material ONMX vesting and lock structures, stakeholder claims, allocation tracking, and the applicable custody or escrow workflows used in the production configuration.

The production Magna infrastructure and onchain records will provide independent evidence of relevant restricted balances and release activity.

## Treasury Reserve & LP — 8 years

The **725,000,000 ONMX Treasury Reserve & LP allocation** is intended to use a long-duration **eight-year** structure through Magna.

The reserve design is intended to provide:

* independent lifecycle infrastructure,
* long-duration supply discipline,
* public onchain verification,
* clearer separation between restricted treasury supply and public float,
* auditable historical releases.

The eight-year structure applies to this 72.5% allocation. It does not mean that every token within the 1 billion ONMX maximum supply follows the same eight-year vesting schedule.

The production Magna deployment and its onchain address will become authoritative for the live restricted balance and release mechanics once activated.

## Team & Advisors — 4 years

The **50,000,000 ONMX Team & Advisors allocation** is intended to vest over **four years** through Magna.

Public supply reporting should show the aggregate Team & Advisors restricted, vested, claimable, and released status without publishing private individual allocation information.

## Seed — 6-month cliff + 18 months

The **25,000,000 ONMX Seed allocation** is structured with:

* a 6-month cliff,
* followed by 18 months of linear vesting,
* monthly claim availability after the cliff under the production implementation.

Individual Seed participants will be able to monitor their own allocation through the Magna stakeholder dashboard after onboarding.

## Public-float reporting

Protocol-reported circulating supply should distinguish whether ONMX is:

* unlocked and publicly available,
* vested but unclaimed,
* claimed and transferable,
* locked or unvested,
* treasury controlled,
* liquidity-pool inventory,
* permanently burned.

This helps users, exchanges, and market-data platforms distinguish fixed maximum supply from actual public float.

## Project-level supply transparency

A private Magna stakeholder account displays the allocations associated with that stakeholder. It should not be treated as the project-wide public supply dashboard.

Onchain Matrix will therefore maintain an aggregate public supply view covering:

* Maximum Supply
* Total Supply
* Circulating Supply
* Locked / Vesting Supply
* Treasury-Controlled Supply
* Treasury Reserve & LP 8-year status
* Team & Advisors 4-year status
* Seed vesting status
* Burned Supply
* Historical releases

If Magna provides a public ONMX project-level supply interface, the official link will be added to this page.

## Supply reporting table

| Metric                     | Reporting Basis                            | Verification                                   |
| -------------------------- | ------------------------------------------ | ---------------------------------------------- |
| Maximum Supply             | 1,000,000,000 ONMX                         | ONMX token contract                            |
| Total Supply               | Current onchain state                      | BscScan + token contract                       |
| Circulating Supply         | Current published methodology              | Onchain records + supply methodology           |
| Locked / Vesting Supply    | Current production lock and vesting state  | Magna / vesting contracts / BscScan            |
| Treasury Reserve & LP      | 725,000,000 ONMX; 8-year structure         | Magna production deployment + BscScan          |
| Team & Advisors            | 50,000,000 ONMX; 4-year vesting            | Magna production allocation + onchain records  |
| Seed                       | 25,000,000 ONMX; 6-month cliff + 18 months | Magna production allocation / vesting contract |
| Treasury-Controlled Supply | Official protocol-controlled balances      | Treasury / multisig / lock contracts           |
| Burned Supply              | Completed burn events                      | Onchain burn transactions                      |

## Treasury releases and market transparency

Onchain Matrix does not publish a mechanical schedule of future treasury market transactions that could create a predictable front-running or shorting target.

Supply transparency remains independently verifiable through:

* lock architecture,
* covered allocation,
* current restricted balance,
* historical releases,
* current treasury-controlled balance,
* executed transfers after they occur,
* material changes in token policy.

The distinction is between verifying supply status and pre-announcing an execution strategy.

## Buyback and burn reporting

Where protocol policy, treasury conditions, market liquidity, legal considerations, and available surplus permit, ONMX can be repurchased and burned.

Completed burn events can be verified onchain and reflected in updated supply reporting.

## Data-provider reconciliation

CoinMarketCap, CoinGecko, exchanges, and other third parties can classify circulating supply differently.

Onchain Matrix's documentation is designed to provide verifiable evidence for independent classification, including allocation tables, Magna vesting and lock infrastructure, treasury addresses, burn transactions, and a clear distinction between restricted balances and public circulation.
