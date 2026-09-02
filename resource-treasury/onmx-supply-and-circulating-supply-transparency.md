# ONMX Supply and Circulating Supply Transparency

ONMX has a fixed total supply of **1,000,000,000 ONMX** on BNB Chain. Supply transparency distinguishes between maximum supply, issued supply, restricted or vesting supply, treasury-controlled supply, burned supply, and tokens reasonably available for public market circulation.

An allocation's economic purpose is not the same as its circulating status.

## Token allocation

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

The Core Treasury Allocation combines token allocations associated with treasury formation and launch capital flows:

**72.5% Treasury Reserve & LP + 10.0% Public Sale + 2.5% Presale + 2.5% Seed = 87.5%.**

This classification describes the intended economic role of these allocations. It does not mean that 87.5% of ONMX is immediately circulating, unlocked, available for sale, or simultaneously deployed.

## Supply categories

### Maximum Supply

The maximum number of ONMX that can exist under the fixed-supply design.

**Maximum Supply: 1,000,000,000 ONMX**

### Total Supply

The amount of ONMX existing onchain after accounting for any permanent supply reductions recognized by the token contract and applicable reporting methodology.

### Circulating Supply

ONMX that is issued and reasonably available for normal public market circulation.

Tokens that remain locked, unvested, unreleased, permanently burned, or otherwise restricted from normal public float are treated separately in protocol reporting.

Market-data providers and exchanges can apply their own circulating-supply methodologies. Their published methodology controls the figure displayed on their platform.

### Locked / Vesting Supply

ONMX subject to a contractual lock, cliff, linear vesting schedule, or other transfer restriction that prevents normal public circulation.

### Treasury-Controlled Supply

ONMX held or controlled for treasury, liquidity, ecosystem, infrastructure, or other protocol purposes. Treasury-controlled supply is not automatically equivalent to circulating public float.

### Burned Supply

ONMX permanently removed from usable supply through the applicable burn mechanism and recognized by the relevant onchain and reporting methodology.

## Treasury Reserve & LP — 72.5%

The **725,000,000 ONMX Treasury Reserve & LP allocation** is intended to use long-duration third-party lock or vesting infrastructure over an **eight-year period**.

**Magna** has been selected as the infrastructure provider for the reserve structure.

The reserve design is intended to provide:

* Independent infrastructure
* Long-duration supply discipline
* Public onchain verification
* Reduced reliance on discretionary internal custody
* Flexibility for treasury deployment without publishing a mechanical schedule of future market transactions

The production Magna deployment and its onchain address become the authoritative source for the live locked balance and release mechanics once activated.

## Seed allocation — 2.5%

The **25,000,000 ONMX Seed allocation** is structured with:

* A 6-month cliff
* Followed by 18 months of linear vesting
* Monthly claim availability after the cliff under the production vesting implementation

The vesting contract and claim interface determine the live unlock and claim state.

## Public-float reporting

Protocol-reported circulating supply distinguishes whether each allocation is:

* Unlocked and publicly available
* Vested but unclaimed
* Claimed but still held in a restricted protocol wallet
* Locked or unvested
* Treasury controlled
* Liquidity-pool inventory
* Permanently burned

This allows users, exchanges, and market-data platforms to distinguish fixed maximum supply from actual public float.

## Supply reporting table

| Metric                     | Reporting basis                                    | Verification                         |
| -------------------------- | -------------------------------------------------- | ------------------------------------ |
| Maximum Supply             | 1,000,000,000 ONMX                                 | ONMX token contract                  |
| Total Supply               | Current onchain state                              | BscScan + token contract             |
| Circulating Supply         | Current published methodology                      | Onchain records + supply methodology |
| Locked / Vesting Supply    | Current lock and vesting state                     | Magna / vesting contracts / BscScan  |
| Treasury-Controlled Supply | Balances of official protocol-controlled addresses | Treasury / multisig / lock contracts |
| Burned Supply              | Completed burn events                              | Onchain burn transactions            |

## Treasury releases and market transparency

Onchain Matrix does not publish a mechanical schedule of future treasury market transactions that could create a predictable front-running or shorting target.

Supply transparency remains independently verifiable through:

* Lock architecture
* Covered allocation
* Current locked balance
* Historical releases
* Current treasury-controlled balance
* Executed transfers after they occur
* Material changes in token policy

The distinction is between verifying supply status and pre-announcing an execution strategy.

## Buyback and burn reporting

Where protocol policy, treasury conditions, market liquidity, legal considerations, and available surplus permit, ONMX can be repurchased and burned.

Completed burn events can be verified through the relevant transaction history and reflected in updated supply reporting.

## Data-provider reconciliation

CoinMarketCap, CoinGecko, exchanges, and other third parties can classify circulating supply differently.

Onchain Matrix's supply documentation is designed to provide verifiable evidence for independent classification, including allocation tables, vesting and lock contracts, treasury addresses, burn transactions, and a clear distinction between restricted balances and public circulation.
