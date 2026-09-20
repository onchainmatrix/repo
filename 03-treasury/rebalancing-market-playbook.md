---
description: Treasury rebalancing, market-response rules, and the volatility allocation playbook.
---

# Rebalancing & Market Playbook

Market conditions change continuously. Onchain Matrix is designed around event- and threshold-based capital management rather than a permanently static allocation.

## Rebalancing principles

Treasury adjustments can be driven by factors such as:

- allocation drift,
- liquidity requirements,
- changing yield conditions,
- strategy risk changes,
- market volatility,
- collateral conditions,
- protocol or counterparty events,
- reserve requirements.

The purpose of automation is to enforce discipline, not to remove oversight.

## Risk-off controls

Treasury policy can reduce or pause exposure when predefined risk conditions are met. Examples can include:

- deteriorating liquidity,
- abnormal oracle behavior,
- smart-contract or protocol incidents,
- excessive portfolio concentration,
- stressed collateral markets,
- breach of strategy limits.

## Volatility allocation playbook

Volatility is not only a risk event. It can create disciplined allocation windows when the treasury remains within risk limits.

A market dislocation can lead to one or more actions:

1. **Preserve liquidity** and reduce unnecessary risk.
2. **Accumulate approved assets selectively** when valuations and liquidity support deployment.
3. **Execute ONMX buybacks** when permitted by policy and when market, treasury, legal, and liquidity conditions are satisfied.
4. **Burn repurchased ONMX** where the applicable token-economics policy calls for supply reduction.
5. **Reposition for recovery** while maintaining reserve and exposure constraints.

## Execution discretion

The protocol should not publish a mechanical schedule that creates a predictable map of future market transactions. Buybacks, treasury deployment, and reallocation remain condition-based and subject to treasury policy.
