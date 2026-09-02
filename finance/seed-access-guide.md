# Seed Access Guide

Onchain Matrix Seed Access is designed to provide permissioned access to the Seed Round before the planned Public Sale / TGE stage.

The Seed Round is intended primarily to form the protocol-owned treasury base.

### Current Seed Structure

| Term                              | Current Structure                                                    |
| --------------------------------- | -------------------------------------------------------------------- |
| Round                             | Seed                                                                 |
| Seed allocation                   | 2.5% of maximum ONMX supply                                          |
| Seed tokens                       | 25,000,000 ONMX                                                      |
| Seed price                        | $0.14 per ONMX                                                       |
| Public Sale / TGE reference price | $0.20 per ONMX                                                       |
| Reference discount                | 30% to the $0.20 reference price                                     |
| Vesting                           | 6-month cliff + 18-month linear vesting                              |
| Claims                            | Monthly after the cliff under the applicable vesting implementation  |
| Primary use of funds              | Treasury formation                                                   |
| Seed capacity                     | $3.5 million                                                         |
| Settlement asset                  | USDT, subject to the live interface and applicable transaction terms |

{% hint style="warning" %}
The Public Sale / TGE reference price is not a guarantee of future market price, liquidity, listing price, or appreciation.
{% endhint %}

## Before You Begin

{% stepper %}
{% step %}
### Use only the official Seed Access page

Begin from the official Onchain Matrix website:

**onchainmatrix.com**

Do not follow Seed-payment instructions sent through unsolicited direct messages, unofficial Telegram accounts, social-media replies, or third-party websites.
{% endstep %}

{% step %}
### Review the live Terms

Seed participation is permissioned.

Eligibility can depend on:

* jurisdiction,
* participant status,
* applicable legal restrictions,
* wallet and access controls,
* technical availability,
* acceptance of the current Terms.

The live Terms and access controls govern participation.

Access to the Seed interface does not itself guarantee eligibility.
{% endstep %}

{% step %}
### Use a wallet you control

Use a compatible self-custody wallet for which you control the keys or recovery mechanism.

Never provide a private key or seed phrase to Onchain Matrix, a community moderator, a support representative, or any website.
{% endstep %}
{% endstepper %}

## Participation Flow

The exact interface can evolve, but the Seed Access process follows the general sequence below.

{% stepper %}
{% step %}
### Access

Open the official Seed Access interface from onchainmatrix.com.

Confirm that:

* the domain is correct,
* the connection is secure,
* you are not following a cloned or sponsored imitation site.
{% endstep %}

{% step %}
### Confirm Eligibility

Complete the eligibility and participation confirmations presented by the live interface.

Participation may be unavailable where applicable restrictions or access controls prevent participation.

Do not attempt to bypass geographic, legal, wallet, or eligibility controls.
{% endstep %}

{% step %}
### Connect Wallet

Connect the wallet that you intend to use for the Seed transaction and future allocation verification.

Before approving any wallet request, confirm:

* the domain,
* the requested network,
* the requested action,
* the contract or spender address where displayed.

A wallet connection request should never require disclosure of your private key or recovery phrase.
{% endstep %}

{% step %}
### Review the Current Terms

Before submitting a transaction, verify the terms displayed by the interface.

Check:

* Seed price,
* amount of ONMX associated with the transaction,
* settlement asset,
* settlement network,
* vesting terms,
* transaction amount,
* applicable restrictions,
* receiving or sale contract details.

{% hint style="warning" %}
If the displayed transaction terms differ materially from the official documentation, do not proceed until the difference is resolved through an official Onchain Matrix channel.
{% endhint %}
{% endstep %}

{% step %}
### Prepare USDT

The current public Seed overview identifies **USDT** as the settlement route.

Use only the supported USDT token and network displayed in the live Seed interface.

Do not send USDT directly to an address unless that transaction route is explicitly provided through the official interface and applicable transaction terms.
{% endstep %}

{% step %}
### Approve the Transaction

If the Seed contract requires a token approval, your wallet may display a separate approval transaction before participation can be completed.

Review the spender address and approval amount before confirming.

Where the wallet supports custom approval limits, avoid granting unnecessary permissions beyond what is required by the transaction.
{% endstep %}

{% step %}
### Confirm Participation

Review the final transaction in your wallet before signing.

Confirm:

* network,
* contract address,
* settlement amount,
* token approval where applicable,
* estimated gas,
* transaction type.

Once submitted, wait for the required blockchain confirmation.
{% endstep %}

{% step %}
### Save Your Transaction Record

Keep a record of:

* transaction hash,
* participating wallet address,
* date,
* settlement amount,
* allocation shown by the interface.

The blockchain transaction hash is an important reference if support is ever required.
{% endstep %}
{% endstepper %}

## Vesting & Claims

Seed allocations are structured with:

**6-month cliff + 18-month linear vesting**

Monthly claim availability begins after the cliff under the applicable vesting implementation.

### During the cliff

The Seed allocation remains subject to the cliff and is not immediately claimable.

### After the cliff

Vesting begins to become claimable according to the applicable linear schedule and contract implementation.

### At TGE

The Seed structure is not designed to provide unrestricted immediate Seed liquidity at TGE.

### Vesting contract verification

When the applicable Seed vesting contract is deployed, its official address and verification link should be published through the Onchain Matrix GitBook.

Use only the vesting interface and contract linked from official Onchain Matrix channels.

## How to Verify Your Allocation

After participating:

1. Confirm the transaction succeeded on the relevant block explorer.
2. Verify that the destination or contract matches the official Seed infrastructure.
3. Retain the transaction hash.
4. Use the official Seed or vesting interface to view allocation status where available.
5. Verify future claim activity onchain.

Do not rely exclusively on screenshots, emails, or direct messages as proof of allocation.

## Common Issues

<details>

<summary>Wallet will not connect</summary>

Confirm that:

* the wallet is supported,
* the correct network is available,
* the browser or wallet extension is current,
* pop-up or connection requests are not being blocked.

</details>

<details>

<summary>Seed Access is unavailable</summary>

Possible reasons can include:

* Seed Access has not yet opened,
* the round has paused or closed,
* eligibility requirements are not satisfied,
* jurisdictional restrictions apply,
* the interface is temporarily unavailable.

</details>

<details>

<summary>Wrong network</summary>

Do not submit a transaction until your wallet is connected to a network supported by the live Seed interface.

</details>

<details>

<summary>USDT balance is not visible</summary>

Confirm that you are viewing the supported USDT contract on the correct network.

Different networks can have different USDT contract addresses.

</details>

<details>

<summary>Transaction remains pending</summary>

Check the transaction on the relevant block explorer.

Network congestion or insufficient gas settings can delay confirmation.

Do not immediately submit duplicate transactions without first checking whether the original transaction is still pending.

</details>

<details>

<summary>Allocation is not claimable</summary>

Seed allocations are subject to the applicable cliff and vesting schedule.

A confirmed Seed transaction does not mean the full ONMX allocation is immediately transferable.

</details>

## Security Checklist

Before every Seed-related transaction:

* Start from **onchainmatrix.com**.
* Verify the current Terms.
* Confirm the connected network.
* Confirm the official contract or destination.
* Confirm the correct USDT token.
* Review transaction details in your wallet.
* Never share a seed phrase or private key.
* Ignore unsolicited payment instructions.
* Do not trust addresses copied only from social media or direct messages.
* Save the transaction hash after completion.

## Important Notice

{% hint style="warning" %}
Seed participation involves digital-asset, smart-contract, market, liquidity, regulatory, operational, and cybersecurity risk.

The $0.20 Public Sale / TGE reference price does not guarantee a future market price.

Vesting does not guarantee future liquidity or token value.

Participants are responsible for confirming eligibility and compliance with the applicable Terms and local law.
{% endhint %}
