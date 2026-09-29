# Shopify Storefront Monitoring for Prices, Stock, and Catalog Changes | Agent Skill

A dated storefront change log by product, variant, and region, with verified price and stock observations.

This public Agent Skill addresses **shopify storefront monitoring** with Magnetic Proxy residential routing where the job requires it. It is an independent use-case package, not an MCP or a claim that the product has completed an authenticated task.

**Product role:** Magnetic Proxy is the routing and observed-location layer for any live regional check in this skill. Without an authorized account and verified exit, the agent may prepare or analyze supplied data but cannot claim a live regional observation. The proxy does not grant data-access rights.

## What you can ask an agent to do

> Track these three public Shopify storefronts weekly for the 250 ml skincare variant in the US and Mexico: displayed price, sale badge, and availability.

**Example result (illustrative, not a live run):** Storefront log: Store A US 250 ml price changed USD 32 → USD 29 with sale badge, confirmed twice. Store B Mexico showed USD market despite a Mexico exit; regional comparison held for review. Store C page was inaccessible; no stock conclusion.

## Install

```bash
npx skills add MagneticProxy/magneticproxy-shopify-storefront-monitoring-skill --skill shopify-storefront-monitoring
```

Or copy this prompt into an agent that supports skill installation:

> Install the `shopify-storefront-monitoring` skill from https://github.com/MagneticProxy/magneticproxy-shopify-storefront-monitoring-skill and use it to help with: [describe your task]. Confirm installation, ask for my authorized inputs, and show me the proposed output before any external action.

Read the [skill instructions](skills/shopify-storefront-monitoring/SKILL.md). The agent needs compatible tools and access to your authenticated account to operate Magnetic Proxy; installation alone does not provide that access.

## Scope and trust

- **Input:** User-approved public storefront URLs, product/variant identifiers, countries, cadence, and the fields that matter.
- **Output:** A dated storefront change log by product, variant, and region, with verified price and stock observations.
- **Product:** [Magnetic Proxy Shopify use case](https://www.magneticproxy.com/use-cases/shopify-proxies) and the [main product skill](https://github.com/MagneticProxy/magneticproxy-residential-proxy-agent-skills).
- **Current verification:** skill format and installation discovery are tested locally. An authenticated live product run has not yet been demonstrated for this repository.

The skill does not authorize purchases, scraping behind access controls, email sending, CRM writes, or publication. Third-party sites and product interfaces can change; the agent must observe the current state and report uncertainty.

## Access and privacy

Check the destination’s terms, access permission, and rate limits before collection. A public URL and a successful proxy connection are not authorization to scrape. Stop on access denials or challenges; do not rotate to evade them. [Magnetic Proxy documentation](https://www.magneticproxy.com/documentation) explains routing and restricted targets.

## Review checklist

1. Does the agent request the right inputs and distinguish this job from the other use cases?
2. Does it make the product step observable and avoid inventing results?
3. Does the output preserve source rows/URLs, time, uncertainty, and a clear decision for the user?

Feedback and improvements can be filed as a GitHub issue in this repository.
