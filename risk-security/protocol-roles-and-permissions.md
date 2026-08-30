# Protocol Roles and Permissions

How authority is separated across treasury custody, protocol operations, risk controls, upgrades, data infrastructure, and emergency response.

Onchain Matrix is designed to reduce dependence on unilateral human control. Sensitive authority should be separated by function, limited to what each role requires, and made publicly observable where doing so does not create unnecessary security risk.

## Core principle

No operational role should automatically have unrestricted authority over every part of the protocol.

The control model is intended to separate:

* custody of treasury capital,
* routine protocol execution,
* risk-policy administration,
* contract upgrades,
* emergency actions,
* oracle and data inputs,
* future credit-market operations.

This separation reduces single-point failure and makes it easier to understand what a compromised role could and could not do.

## Role framework

| Role                               | Intended responsibility                                 | Typical permitted actions                                                                      | Intended limitations                                                                                                        |
| ---------------------------------- | ------------------------------------------------------- | ---------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Treasury Multi-Sig                 | Critical treasury custody and high-impact approvals     | Approve treasury actions, administrative transactions, ownership changes where authorized      | No single signer should be able to act alone; signer identities and recovery material are not public operational data       |
| Treasury Operations / Automation   | Execute approved treasury policy                        | Rebalance or deploy capital within approved strategies, limits, and controls                   | Cannot exceed approved exposure limits or independently rewrite treasury policy                                             |
| Risk Administration                | Maintain approved risk parameters                       | Adjust supported limits, caps, collateral parameters, or restrictions within authorized ranges | Should not provide unrestricted custody or withdrawal authority                                                             |
| Upgrade / Administrative Authority | Manage controlled contract changes                      | Execute approved upgrades or configuration changes                                             | High-impact changes should follow defined approvals and delays where implemented                                            |
| Emergency Control                  | Reduce damage during abnormal events                    | Pause or restrict supported activity where technically available                               | Emergency authority should be narrow, observable, and governed by the same custody discipline as other privileged actions   |
| Oracle / Data Infrastructure       | Supply or validate external data used by protocol logic | Provide market prices, valuation inputs, or other approved data                                | Data providers should not control treasury custody; bad or stale data should be subject to validation and fallback controls |
| Credit-Market Roles                | Operate future collateralized-credit infrastructure     | Origination, servicing, monitoring, resolution, or pool functions as implemented               | Powers depend on the specific credit contract and should be documented before launch                                        |

The exact production addresses and permissions for implemented roles should be published in **Deployments & Contract Addresses** when live.

## Treasury custody

Critical treasury authority is designed around multi-party authorization rather than a single wallet or private key.

Treasury custody should provide:

* multiple independent approvals for sensitive actions,
* auditable transaction history,
* separation between proposal and execution where practical,
* restricted administrative access,
* controlled signer changes,
* operational procedures that do not expose sensitive recovery information.

Public transparency should focus on the controlling address, approval structure, and executed actions—not the personal identities or security details of individual signers.

## Routine execution vs. policy authority

Routine capital management and high-level policy are different functions.

Treasury automation or operating wallets may be permitted to execute activity within predefined constraints. Examples can include approved allocation ranges, supported strategies, liquidity limits, or risk thresholds.

They should not automatically be able to:

* remove treasury-wide limits,
* add arbitrary high-risk strategies,
* transfer unrestricted treasury capital,
* change critical ownership,
* bypass emergency or upgrade controls.

The purpose of automation is to enforce disciplined execution, not to create unlimited autonomous authority.

## Risk administration

Risk administration governs the conditions under which capital may be exposed.

Potential controls can include:

* collateral eligibility,
* LTV thresholds,
* debt ceilings,
* borrower or pool caps,
* strategy exposure limits,
* liquidity requirements,
* oracle safeguards,
* market-response thresholds.

Risk roles should be able to reduce or constrain risk without automatically gaining unrelated treasury-custody powers.

## Upgrade authority

Upgradeable infrastructure can be useful during early protocol deployment, but upgrade authority is itself a material risk.

{% stepper %}
{% step %}
### Proposed through an authorized path

High-impact changes should be proposed through an authorized path.
{% endstep %}

{% step %}
### Reviewed and approved

Changes should be reviewed and approved under the applicable control structure.
{% endstep %}

{% step %}
### Delayed where implemented

Changes should be delayed where a timelock or execution delay is implemented.
{% endstep %}

{% step %}
### Executed transparently onchain

Changes should be executed transparently onchain.
{% endstep %}

{% step %}
### Reflected in the deployment registry

Changes should be reflected in the deployment registry.
{% endstep %}
{% endstepper %}

As contracts mature, upgrade authority can be reduced, constrained, or disabled where technically appropriate.

## Emergency authority

Emergency controls exist to reduce potential damage during abnormal conditions, not to provide a general-purpose administrative shortcut.

Depending on the relevant contract, emergency actions may include:

* pausing new activity,
* restricting selected operations,
* reducing exposure,
* disabling an affected integration,
* blocking a compromised execution path.

Emergency authority should remain as narrow as technically practical and should not bypass multi-party custody for unrelated treasury transfers.

## Oracle and data permissions

Price and data infrastructure can influence valuations, collateral health, liquidation behavior, and treasury reporting.

Oracle and data roles should therefore be separated from asset custody and should operate under independent validation, staleness, deviation, and fallback controls where applicable.

See **Oracle & Data Framework** for the protocol's data-control principles.

## Public accountability

For privileged roles that exist onchain, the protocol should publish enough information to allow independent review of:

* the controlling address,
* the role or permission granted,
* the contract to which the permission applies,
* material changes to that permission,
* executed privileged actions.

Sensitive credentials, signer identities, recovery material, and internal infrastructure details should not be published merely for transparency.

## Roles can evolve

The role model will evolve as treasury automation, credit markets, tokenized debt, and security infrastructure mature.

The live contracts and current role registry should take precedence over architectural descriptions if the implementation changes.
