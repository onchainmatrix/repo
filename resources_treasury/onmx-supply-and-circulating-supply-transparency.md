# ONMX Supply and Circulating Supply Transparency

How Onchain Matrix distinguishes maximum supply, allocation, locked or vesting supply, treasury-controlled supply, burned supply, and circulating supply.

ONMX has a fixed total supply of **1,000,000,000 ONMX**. No additional ONMX is intended to be minted beyond the fixed supply.

Supply transparency matters because an allocation's economic purpose is not the same thing as its circulating status.

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

Onchain Matrix identifies the following allocations as the **Core Treasury Allocation**:

**72.5% Treasury Reserve & LP + 10.0% Public Sale + 2.5% Presale + 2.5% Seed = 87.5%**

This classification describes the intended economic role of the allocations in treasury formation and launch capital flows.

{% hint style="info" %}
It does **not** mean that 87.5% of ONMX is immediately circulating, unlocked, available for sale, or simultaneously deployed.
{% endhint %}

## Supply categories

### Maximum Supply

The maximum number of ONMX that can exist under the fixed-supply design.

**Maximum Supply: 1,000,000,000 ONMX**

### Total Supply

The number of ONMX that exists onchain, less tokens that have been permanently burned where the token contract and applicable data provider treat burns as reducing total supply.

### Circulating Supply

For protocol reporting, circulating supply should represent ONMX that is issued and reasonably available for public market circulation, excluding tokens that remain locked, unvested, unreleased, permanently burned, or otherwise restricted in a manner that removes them from normal public float.

Third-party data providers such as exchanges, market-data platforms, and index providers can apply their own circulating-supply methodologies. Their published methodology controls the figure displayed on their platform.

### Locked / Vesting Supply

ONMX subject to a contractual lock, cliff, linear vesting schedule, or other transfer restriction that prevents normal public circulation.

### Treasury-Controlled Supply

ONMX held or controlled for treasury, liquidity, ecosystem, infrastructure, or other protocol purposes. Treasury-controlled supply is not automatically equivalent to circulating public float.

### Burned Supply

ONMX permanently sent to an irrecoverable burn mechanism or otherwise removed from supply according to the token contract and the relevant reporting methodology.

## Treasury Reserve & LP — 72.5%

The **725,000,000 ONMX Treasury Reserve & LP allocation** is intended to use long-duration third-party lock or vesting infrastructure over an **eight-year period**.

The purpose is to provide:

* independent infrastructure,
* long-duration supply discipline,
* public onchain verification,
* reduced reliance on discretionary internal custody,
* flexibility for treasury deployment without publishing a simple fixed schedule of future market sales.

**Selected infrastructure provider:** coming soon

Release and deployment mechanics remain subject to the actual production lock structure, treasury policy, market conditions, protocol requirements, and published terms.

## Seed allocation — 2.5%

The **25,000,000 ONMX Seed allocation** is structured with:

* a 6-month cliff,
* followed by 18 months of linear vesting,
* monthly claim availability after the cliff under the applicable vesting implementation.

The live vesting contract and claim interface should be linked from this page once production deployment is complete.

## Other allocations

The final unlock, vesting, custody, and transfer status of Team & Advisors, Presale, Public Sale, Community Participation, Ecosystem Growth, and Infrastructure Development should be determined from:

1. the applicable production contracts,
2. current token-sale or participation terms,
3. current official tokenomics documentation,
4. public onchain records.

## Public-float reporting

To make supply reporting easier to verify, Onchain Matrix should publish a supply table that can be updated as the token lifecycle evolves.

| Metric                     |                           Amount | Verification                            |
| -------------------------- | -------------------------------: | --------------------------------------- |
| Maximum Supply             |               1,000,000,000 ONMX | Token contract                          |
| Total Supply               |        Update from onchain state | BscScan / token contract                |
| Circulating Supply         | Update using current methodology | Onchain records + published methodology |
| Locked / Vesting Supply    |      Update as contracts go live | Magna / vesting contracts / BscScan     |
| Treasury-Controlled Supply |   Update from official addresses | Treasury / multisig / lock contracts    |
| Burned Supply              |         Update after burn events | Onchain burn transactions               |

## Circulating-supply methodology

When calculating a protocol-reported circulating figure, the methodology should identify whether each allocation is:

* unlocked and publicly available,
* vested but unclaimed,
* claimed but still held by a restricted protocol wallet,
* locked or unvested,
* treasury controlled,
* liquidity-pool inventory,
* burned.

This makes it possible for market-data platforms and users to understand the difference between **fixed supply**, **issued supply**, **restricted supply**, and **public float**.

## Treasury releases and market transparency

Onchain Matrix does not intend to publish a mechanical schedule of future treasury market transactions that could create a predictable front-running or shorting target.

That does not prevent supply transparency.

The protocol can disclose:

* the lock architecture,
* covered allocation,
* current locked balance,
* historical releases,
* current treasury-controlled balance,
* executed transfers after they occur,
* material changes in token policy.

The distinction is between **verifying supply status** and **pre-announcing an execution strategy**.

## Buyback and burn reporting

Where protocol policy, treasury conditions, market liquidity, legal considerations, and available surplus permit, ONMX may be repurchased and burned.

Completed burn events should be published with:

* amount of ONMX burned,
* date,
* transaction hash,
* updated burned supply,
* updated total or circulating supply where applicable.

## Verification sources

Supply reporting should be cross-checkable using:

* the ONMX token contract,
* BscScan,
* treasury and multisig addresses,
* Magna or other applicable lock infrastructure,
* seed and other vesting contracts,
* liquidity contracts,
* burn transactions,
* official Onchain Matrix GitBook updates.

## Data-provider reconciliation

CoinMarketCap, CoinGecko, exchanges, and other third parties can classify circulating supply differently.

When submitting or updating ONMX supply information, Onchain Matrix should provide those platforms with:

* allocation tables,
* vesting and lock contracts,
* treasury addresses,
* burn addresses or transactions,
* public verification links,
* a clear explanation of which balances are restricted from public circulation.

The objective is not to force a particular classification. It is to provide enough verifiable evidence for each platform to apply its methodology accurately.
