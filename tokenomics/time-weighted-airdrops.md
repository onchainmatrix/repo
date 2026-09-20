---
hidden: true
---

# Time-Weighted Airdrops

Onchain Matrix is designed to reward sustained participation without relying on inflationary emissions, short-term farming incentives, or easily manipulated balance snapshots.

When approved, stablecoin airdrops may be funded from a portion of the Treasury Engine’s realized net yield. Eligibility and allocation would be calculated using a time-weighted balance model rather than a single snapshot.

### Airdrop Principles

* Airdrops may come only from realized net distributable treasury yield.
* Treasury principal will not be used to fund airdrops.
* ONMX will not be created or issued to fund airdrops.
* Capital reserves, operating requirements, risk buffers, taxes, fees, and other obligations will be accounted for first.
* Airdrops are variable and discretionary. No amount, payment date, or fixed annual percentage yield is guaranteed.
* The anticipated airdrop cadence is quarterly, subject to realized performance, available reserves, eligibility requirements, and formal approval.
* Treasury Reserve, team and advisor, protocol-owned, liquidity-management, and other designated non-circulating allocations will be excluded.

### 90-Day Time-Weighted Balance

Each eligible participant’s allocation would be based on their average eligible ONMX balance over the applicable 90-day measurement period.

This approach rewards both the number of eligible ONMX held and the duration for which they were held. It also reduces the benefit of purchasing immediately before an airdrop.

Assuming the wallet maintains a constant balance during the stated period:

| Time held during the 90-day period | Approximate weighting |
| ---------------------------------: | --------------------: |
|                            90 days |                  100% |
|                            60 days |                 66.7% |
|                            45 days |                   50% |
|                            30 days |                 33.3% |
|                             7 days |                  7.8% |
|                              1 day |                  1.1% |

There is no rigid 90-day minimum holding requirement. A participant entering during a measurement period may participate proportionally from the date their eligible balance is first recorded.

If a participant increases, reduces, or sells their balance during the period, the calculation reflects the amount held on each day. For example, ONMX held for the first half of the period and sold afterward would contribute only for the days during which it was held.

### Airdrop Calculation

An eligible participant’s share of an approved airdrop would be calculated as:

$$
\text{Airdrop Share} =
\frac{\text{Participant’s Average Eligible ONMX Balance}}
{\text{Total Average Eligible ONMX Balance}}
$$

The participant’s stablecoin airdrop would then be:

$$
\text{Participant Airdrop} =
\text{Approved Airdrop Pool} \times \text{Airdrop Share}
$$

“Average eligible balance” means the time-weighted balance recorded throughout the complete measurement period—not the balance held on one selected date.

### Seed and Presale Allocations

Verified seed and presale allocations may begin accumulating time-based eligibility from the date the allocation is confirmed, even when the corresponding ONMX remains subject to vesting or is not yet transferable before TGE.

Before tokens become transferable, eligibility would be calculated from verified allocation records maintained by Onchain Matrix and its approved vesting or airdrop provider. After tokens are delivered or claimed onchain, the calculation would transition to the participant’s eligible onchain balance without double counting the same tokens.

Participation remains subject to the applicable offering terms, vesting schedule, jurisdictional restrictions, identity and wallet verification, and legal or compliance requirements.

### Wallet Transfers

Holding history is attached to the balance recorded for an eligible wallet and does not automatically transfer to another wallet.

When ONMX is transferred:

* The sending wallet receives weighting only for the balance and period recorded before the transfer.
* The receiving wallet begins accumulating weighting from the time the ONMX is received.
* Transfers between wallets controlled by the same participant do not create additional weighting or duplicate eligibility.
* Administrative wallet migrations may be reviewed separately where ownership can be verified.

### Framework Summary

| Component                          | Proposed structure                                                                                  |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- |
| Airdrop cadence                    | Quarterly, when approved                                                                            |
| Measurement period                 | 90 days                                                                                             |
| Calculation method                 | Time-weighted average eligible balance                                                              |
| Minimum holding period             | None                                                                                                |
| Airdrop asset                      | Stablecoin                                                                                          |
| Funding source                     | Realized net distributable treasury yield                                                           |
| Fixed APY                          | None                                                                                                |
| Treasury principal used            | No                                                                                                  |
| Inflationary ONMX emissions        | No                                                                                                  |
| Pre-TGE seed and presale treatment | Verified allocations may accumulate time-based eligibility                                          |
| Excluded balances                  | Treasury Reserve, team and advisor, protocol-owned and other designated non-circulating allocations |
| Wallet transfers                   | Previous holding history does not automatically transfer                                            |
| Final approval                     | Subject to treasury, legal, compliance, technical, and jurisdictional review                        |

This framework describes a proposed airdrop methodology only. It does not create a guaranteed entitlement to income, establish a fixed return, or require Onchain Matrix to approve an airdrop for any particular period.
