# ONMX Token Contract and Supply Mechanics

ONMX is the ecosystem alignment token of Onchain Matrix, deployed on BNB Chain as a BEP-20 token.

## Token identity

| Property                      | Current specification                        |
| ----------------------------- | -------------------------------------------- |
| Token                         | Onchain Matrix                               |
| Ticker                        | ONMX                                         |
| Network                       | BNB Chain                                    |
| Standard                      | BEP-20                                       |
| Fixed Maximum Supply          | 1,000,000,000 ONMX                           |
| Token Address                 | `0x0D60CC169b26be7fCcf0dEcB3B1Ee337fc5cbE5C` |
| Inflationary Reward Emissions | None in the protocol economic model          |

## Fixed-supply model

The 1,000,000,000 ONMX supply is a maximum supply ceiling, not a statement that the entire supply is circulating.

The protocol distinguishes between:

* Maximum supply
* Total supply
* Economically released supply
* Locked or vesting supply
* Treasury-controlled supply
* Circulating public float
* Burned supply

## Capital-linked supply release

ONMX supply is structured around capital formation and protocol use rather than recurring inflationary emissions.

Token allocations can enter circulation through defined mechanisms such as:

* Sale and capital-formation events
* Vesting completion
* Approved ecosystem or infrastructure use
* Liquidity formation
* Treasury-policy releases

The production contracts and current onchain state determine the actual released and circulating balance.

## Vesting and lock mechanics

Long-duration or restricted allocations are separated from public float through production vesting or lock infrastructure. Onchain Matrix has selected Magna, powered by Kraken, for material ONMX lifecycle infrastructure.&#x20;

The 72.5% Treasury Reserve & LP allocation is intended to use an eight-year structure. Team & Advisors, representing 5% of maximum supply, are intended to vest over four years. Seed follows a six-month cliff followed by eighteen months of linear vesting, with monthly claim availability after the cliff.&#x20;

The applicable production contracts and Magna allocation state determine the actual restricted, vested, claimable, released, and circulating balances.

## No ONMX reward inflation

Treasury yield and protocol revenue are designed to come from productive capital deployment and protocol activity rather than minting new ONMX as recurring rewards.

This separates protocol yield from token issuance.

## Buyback and burn

Where treasury policy, surplus revenue, market liquidity, legal considerations, and protocol conditions permit, ONMX can be repurchased from the market and removed through the applicable burn mechanism.

A completed burn is an onchain event and can be reflected in public supply reporting.

{% hint style="info" %}
Buybacks and burns are condition-based and are not guaranteed.
{% endhint %}

## Stablecoin distributions

Eligible stablecoin-based distributions can be used where permitted and implemented. These distributions are designed to avoid creating new ONMX emissions.

Eligibility, timing, amount, and implementation remain subject to protocol policy, treasury conditions, legal requirements, and the applicable distribution mechanism.

## Verification

Token supply and distribution claims are designed to be cross-checkable using:

* The ONMX token contract
* BscScan
* Official treasury addresses
* Magna or other applicable lock infrastructure
* Vesting contracts
* Liquidity contracts
* Burn transactions
* The current Onchain Matrix supply methodology
