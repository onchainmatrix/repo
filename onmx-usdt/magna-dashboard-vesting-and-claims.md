# Magna Dashboard Vesting and Claims

ONMX Seed vesting and claims are intended to use **Magna** once the applicable production vesting infrastructure is active.

Magna provides a stakeholder dashboard where an eligible ONMX participant can monitor the participant's own allocation and claim tokens when the applicable vesting schedule makes them claimable.

## When can I access Magna?

You can access Magna only after Onchain Matrix has added the email address or wallet associated with your allocation to the Magna platform.

If Magna does not recognize your email or wallet, first confirm with Onchain Matrix that your stakeholder record has been added.

## How to log in

Go to the official Magna stakeholder application:

**app.magna.so**

Magna currently supports stakeholder login methods including:

* one-time email Magic Link,
* supported EVM wallet,
* WalletConnect-compatible wallet,
* Google login for supported Google-managed accounts.

Use the email address or wallet associated with your ONMX allocation.

For additional account protection, enable multi-factor authentication where available.

## Your ONMX portfolio

After logging in, the Magna portfolio displays the assets and allocations associated with your stakeholder account.

For an ONMX allocation, the dashboard can display fields such as:

### Allocated

The total ONMX assigned to the allocation.

### Unlocked

The amount of ONMX that has reached its applicable unlock point to date.

### Releasable

Where an allocation contains both unlock and vesting conditions, this reflects the amount that satisfies the applicable release conditions.

### Funded

The amount of ONMX funded into the relevant vesting contract or transfer flow.

### Claimable

The amount currently available for the stakeholder to claim.

### Received

The amount already received by the stakeholder.

## Allocation details

Opening an individual ONMX allocation can provide additional information such as:

* allocation category,
* total ONMX allocation,
* allocation status,
* wallet on record,
* vesting or unlock terms,
* visual timeline,
* individual release dates,
* claim or withdrawal history.

The production Magna record and onchain vesting contract determine the live allocation status.

## Seed vesting schedule

ONMX Seed allocations are structured as:

**6-month cliff + 18-month linear vesting**

Monthly claim availability begins after the cliff under the production implementation.

### During the cliff

The Seed allocation remains subject to the cliff. A completed Seed purchase does not mean the allocation is immediately claimable.

### After the cliff

ONMX becomes eligible for release according to the applicable linear schedule.

The dashboard can show the participant's current unlocked and claimable amount as the schedule progresses.

## How to claim ONMX

When ONMX is available to claim, Magna displays a **Claim** action for the applicable allocation.

{% stepper %}
{% step %}
## Log in

Log in with the email or wallet associated with the ONMX allocation.
{% endstep %}

{% step %}
## Open the ONMX allocation

Open the ONMX allocation.
{% endstep %}

{% step %}
## Confirm claim availability

Confirm that the allocation status shows tokens available to claim.
{% endstep %}

{% step %}
## Select Claim

Select **Claim**.
{% endstep %}

{% step %}
## Connect a wallet

Connect a wallet to sign the claim transaction.
{% endstep %}

{% step %}
## Review the transaction

Review the transaction.
{% endstep %}

{% step %}
## Sign and submit

Sign and submit.
{% endstep %}

{% step %}
## Confirm the transaction

Confirm the transaction through the relevant block explorer.
{% endstep %}
{% endstepper %}

Under Magna's current claim flow, the wallet signing the claim transaction can be different from the receiving allocation wallet, but the claimed tokens are delivered to the allocation wallet on record.

{% hint style="warning" %}
Always verify the live Magna interface and production ONMX contract before signing.
{% endhint %}

## Wallet on record

The wallet associated with an ONMX allocation is important because it determines where claimed tokens are delivered.

Before the allocation is activated onchain, confirm that the correct compatible wallet is associated with the allocation.

Changes to an active claim allocation can be restricted after the allocation has started onchain.

If the wallet on record is incorrect, contact Onchain Matrix support through an official channel before attempting a claim.

## Claim status

Magna can display allocation states such as:

* Not Started
* Claim Available
* Up To Date
* Completed
* Missing Wallet
* Pending Funding
* other states applicable to the production distribution configuration.

A Seed allocation can be valid even when no Claim button is available yet. The claim function appears only when the applicable conditions are satisfied and the production allocation is funded and claimable.

## What you will not see in your private Magna account

Your stakeholder dashboard is intended to show **your own ONMX allocations**.

It should not be treated as a public view of individual Team, Advisor, Seed, Treasury, or other stakeholder allocations.

For project-wide supply transparency, use the official Onchain Matrix public supply documentation.

## Project-wide ONMX supply view

The public Onchain Matrix supply view will show the aggregate ONMX structure, including:

* 1,000,000,000 ONMX maximum supply,
* Treasury Reserve & LP — 72.5% / 725,000,000 ONMX,
* Treasury Reserve & LP — 8-year Magna structure,
* Team & Advisors — 5% / 50,000,000 ONMX,
* Team & Advisors — 4-year Magna vesting,
* Seed — 2.5% / 25,000,000 ONMX,
* Seed — 6-month cliff + 18-month vesting,
* circulating supply,
* locked / vesting supply,
* treasury-controlled supply,
* burned supply,
* historical releases where applicable.

This public view is designed to provide transparency without exposing private stakeholder identities.

If a public Magna project-level dashboard becomes available for ONMX, the official link will be published through the GitBook.

## Troubleshooting

<details>

<summary>I cannot log in</summary>

Confirm that Onchain Matrix has already added the email address or wallet associated with your allocation to Magna.

Also confirm that you are using **app.magna.so**.

</details>

<details>

<summary>My allocation is visible but I cannot claim</summary>

Possible reasons include:

* the cliff has not ended,
* no ONMX is currently claimable,
* the allocation is pending funding,
* the production vesting transaction has not yet been completed,
* the interface is still indexing an onchain transaction.

</details>

<details>

<summary>My claim transaction is pending</summary>

Check the transaction on the relevant block explorer before submitting another transaction.

</details>

<details>

<summary>I claimed ONMX but do not see it in my wallet</summary>

Confirm the transaction succeeded and that your wallet recognizes the official ONMX token contract.

Some wallets require the token contract to be added manually before the balance is displayed.

</details>

## Security

{% hint style="danger" %}
Magna, Onchain Matrix, and legitimate support personnel will never require your private key or recovery phrase.
{% endhint %}

Before signing a claim:

* confirm the Magna domain,
* confirm the network,
* confirm the ONMX contract,
* verify the receiving allocation wallet,
* inspect the transaction in your wallet,
* confirm the transaction on the relevant block explorer after execution.

## Source of truth

The production vesting contract, current onchain state, and Magna allocation record are authoritative for claimable balances and completed claims.

Documentation describes the intended structure but does not override the production contracts.
