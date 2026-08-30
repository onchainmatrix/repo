# Security Center

A central reference for Onchain Matrix security controls, review status, responsible disclosure, incident response, and public security evidence.

For a protocol designed to manage capital, security is not a separate feature. It is part of custody, contracts, infrastructure, access control, monitoring, upgrades, and operational procedures.

## Security model

Onchain Matrix is designed around multiple layers of control:

1. **Multi-party treasury custody** — critical treasury authority requires multiple approvals rather than unilateral control.
2. **Privileged access security** — administrative access is permissioned, segmented, and minimized.
3. **Smart-contract security** — core contracts follow structured development, testing, verification, review, and deployment procedures.
4. **Controlled upgrades** — high-impact changes use defined approval paths and delay mechanisms where implemented.
5. **Monitoring** — contract events, privileged actions, treasury movements, infrastructure alerts, oracle issues, and abnormal protocol behavior can be monitored.
6. **Emergency response** — protective controls can restrict activity where technically appropriate during a security event.

{% hint style="info" %}
No security architecture can eliminate all risk. The objective is to reduce attack surface, limit authority, increase detection, and improve the protocol's ability to respond to abnormal conditions.
{% endhint %}

## Security status

| Area                             | Current documentation status                                               |
| -------------------------------- | -------------------------------------------------------------------------- |
| Multi-signature treasury control | Part of the protocol security architecture                                 |
| Public contract verification     | Required for production deployments where supported                        |
| Controlled upgrade procedures    | Part of the protocol design                                                |
| Monitoring and incident response | Part of the operational security model                                     |
| External audit reports           | Publish here as completed                                                  |
| Public bug bounty                | Do not assume active unless explicitly listed here                         |
| Incident history                 | Publish material incidents and post-incident information where appropriate |

{% hint style="warning" %}
Until an external audit report is published through an official Onchain Matrix channel, users should not assume that a particular contract has been externally audited.
{% endhint %}

## Smart-contract security lifecycle

Production smart contracts should move through a disciplined lifecycle that can include:

* specification and architecture review,
* threat modeling,
* unit and integration testing,
* permission and role review,
* edge-case and failure-mode testing,
* static or automated analysis where appropriate,
* internal review,
* external review or audit for material contracts,
* source-code verification after deployment,
* post-deployment monitoring.

{% hint style="warning" %}
Security review does not guarantee that a contract is free of vulnerabilities.
{% endhint %}

## Audit and review registry

Published security reports should be listed here in a consistent format.

| Component                     | Reviewer                   | Review type                                           | Date | Report                                                | Status                     |
| ----------------------------- | -------------------------- | ----------------------------------------------------- | ---- | ----------------------------------------------------- | -------------------------- |
| ONMX Token                    | —                          | —                                                     | —    | Publish when available                                | Not listed                 |
| Seed / Sale Contracts         | —                          | —                                                     | —    | Publish when available                                | Not listed                 |
| Vesting / Lock Infrastructure | Third-party infrastructure | Provider security information + implementation review | —    | Publish relevant links when live                      | Implementation stage       |
| Treasury Automation           | —                          | —                                                     | —    | Publish before or as material automation is activated | Roadmap / activation stage |
| Credit Contracts              | —                          | —                                                     | —    | Publish before or with production launch              | Roadmap                    |
| Pool / Marketplace Contracts  | —                          | —                                                     | —    | Publish before or with production launch              | Roadmap                    |

Only completed, publicly accessible reviews should be represented as completed audits.

## Responsible disclosure

Security researchers who identify a potential vulnerability should use the official contact method published by Onchain Matrix.

Until a dedicated security-disclosure channel is published, use only the contact route listed on the official Onchain Matrix website or documentation.

A vulnerability report should ideally include:

* affected contract, interface, or system,
* network and address where applicable,
* technical description,
* reproduction steps or proof of concept,
* potential impact,
* recommended mitigation if known,
* a secure way to contact the researcher.

Researchers should avoid publicly disclosing an exploitable issue before the protocol has had a reasonable opportunity to investigate and mitigate it.

## Bug bounty

A public bug-bounty program should be linked here if and when activated.

{% hint style="warning" %}
The absence of a published bounty should not be interpreted as permission to exploit a vulnerability or access systems without authorization.
{% endhint %}

## Monitoring

Security monitoring can cover:

* treasury movements,
* multisig and privileged transactions,
* contract ownership or implementation changes,
* abnormal contract events,
* unexpected protocol-state changes,
* oracle anomalies,
* infrastructure authentication events,
* service health and availability,
* suspicious interaction patterns.

Monitoring should focus on actionable signals without exposing sensitive internal infrastructure or operational procedures.

## Incident response

If a material security event occurs, response actions can include, where technically and operationally appropriate:

{% stepper %}
{% step %}
## Identify and validate the event
{% endstep %}

{% step %}
## Restrict the affected activity
{% endstep %}

{% step %}
## Protect unaffected capital and infrastructure
{% endstep %}

{% step %}
## Preserve logs and onchain evidence
{% endstep %}

{% step %}
## Investigate scope and root cause
{% endstep %}

{% step %}
## Remediate or upgrade affected systems under the applicable approval process
{% endstep %}

{% step %}
## Restore activity only after validation
{% endstep %}

{% step %}
## Publish material information when doing so no longer creates additional security risk
{% endstep %}
{% endstepper %}

Emergency powers are themselves sensitive and should remain subject to controlled custody and access principles.

## Public security evidence

Security claims should be tied to evidence wherever practical. Useful evidence can include:

* verified deployed contracts,
* multisig transactions,
* role and permission data,
* timelock activity,
* published audit reports,
* security-review reports,
* onchain events,
* documented deployment procedures,
* incident reports.

## User security checklist

Before interacting with Onchain Matrix:

* use the official website and GitBook,
* verify the network before signing,
* confirm the contract address against **Deployments & Contract Addresses**,
* verify the address on the relevant block explorer,
* do not trust unsolicited direct messages,
* do not share seed phrases or private keys,
* review transaction permissions before signing,
* confirm that a product marked as roadmap is actually live before interacting with any claimed deployment.
