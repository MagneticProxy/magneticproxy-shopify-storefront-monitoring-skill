# Shopify Price and Stock Monitoring with Magnetic Proxy

A dated storefront change log by product, variant, and region, with verified price and stock observations. This Agent Skill helps **ecommerce and merchandising teams observing public shopify competitor storefronts** prepare an evidence-based result using Magnetic Proxy for authorized residential routing and regional observations.



## What you get

- Track price and availability wording for exact Shopify variants
- Find changes in catalog, promotions and regional storefront experience
- Distinguish unavailable pages from actual out-of-stock signals

Start with [the worked example](skills/shopify-storefront-monitoring/references/worked-example.md), the [deliverable template](skills/shopify-storefront-monitoring/assets/deliverable-template.md) and the [output columns](skills/shopify-storefront-monitoring/assets/output.csv).

## Install and start

Copy this prompt into an agent that supports skill installation:

> Review and install `shopify-storefront-monitoring` from https://github.com/MagneticProxy/magneticproxy-shopify-storefront-monitoring-skill and the `magneticproxy` product skill from https://github.com/MagneticProxy/magneticproxy-residential-proxy-agent-skills. Confirm which files were installed and whether you can operate my browser or product account. Help me with: [my task]. Use existing capacity first; guide signup or recommend a suitable current plan when needed, and obtain my approval before a paid purchase. Start with a bounded sample and show the observed results and unresolved work.

Or use the Skills CLI from your project folder:

```bash
npx skills add MagneticProxy/magneticproxy-shopify-storefront-monitoring-skill --skill shopify-storefront-monitoring
npx skills add MagneticProxy/magneticproxy-residential-proxy-agent-skills --skill magneticproxy
```

Select your agent when prompted. For a non-interactive installation, add the appropriate agent flag, for example `--agent codex` or `--agent claude-code`. Review installed instructions and scripts before running them. Installation does not grant browser tools, credentials or a subscription. A plain chat can read the instructions but may not install or operate the product.

The complete skill folder is the canonical package, including references and templates. A lone downloaded `SKILL.md` omits those files; use the repository installation or copy the complete folder into your agents supported skills directory. An MCP is not required or assumed.

## From install to first useful result

1. **Install and connect.** Install this skill and the `magneticproxy` product skill. Confirm your agent has browser/computer control or an authorized proxy client; installation alone provides no account access.
2. **Log in or sign up.** Open [Magnetic Proxy](https://app.magneticproxy.com/#/my-proxies). Reuse your account; otherwise use the visible Sign up flow. Complete authentication yourself without pasting credentials into the conversation.
3. **Choose capacity for the job.** Inspect available Capsules and GB. For ongoing offer monitoring, assess Price Monitoring; for authorized campaign landing QA, assess General Purpose Premium. Start with existing suitable capacity. If capacity is insufficient, compare [current plans](https://www.magneticproxy.com/pricing) and recommend the smallest suitable option from observed pilot usage. Follow its current Choose Plan checkout link; do not hardcode a price, discount or checkout token.
4. **Approve any purchase.** Show Capsule, capacity, billing period and current cost before purchase. Continue paid checkout only when the user explicitly authorizes that transaction. A skill installation is not purchase approval.
5. **Prove the route.** Configure the current product, verify the exit in the same browser/client and run a bounded permitted sample. Expand only within the agreed scope. If the approved data route does not need a proxy, explain that and do not invent a purchase requirement.

## Try this task

> Track these three public Shopify storefronts weekly for the 250 ml skincare variant in the US and Mexico: displayed price, sale badge, and availability.

**Bring:** User-approved public storefront URLs, product/variant identifiers, countries, cadence, and the fields that matter.

**Illustrative result:** Mark the blue variant inaccessible and comparison pending. Do not report it sold out or compare it with red. Retain the earlier observation with its timestamp.

Read the [complete workflow](skills/shopify-storefront-monitoring/SKILL.md) for source access, execution and decision rules.

## Common questions

### Can it read Shopify inventory quantities or private admin data?

A storefront observation can show displayed availability, not an authoritative stock count. Private merchant APIs require separate authorization and current API documentation.

### Why use Magnetic Proxy here?

Magnetic Proxy provides the configured geographic connection for permitted live regional checks. The skill adds comparable observations and a decision-ready deliverable. Supplied-data analysis can proceed without pretending that a live proxy check occurred.

### Is signup or a paid plan required?

An account is required to operate the product. Use available account capacity first. A paid plan is needed only when the requested operation requires capacity or features the account does not have; consult the current product pricing. Installing this repository does not start a paid subscription.

### Has the live workflow been verified?

Repository validation and installation checks cover packaging; the worked example uses synthetic inputs. A live workflow requires an authenticated account, an approved sample and an observed final result. See [QA and maintenance](QA.md) for the exact boundary.

## Access and privacy

Check the destination’s terms, access permission, and rate limits before collection. A public URL and a successful proxy connection are not authorization to scrape. Stop on access denials or challenges; do not rotate to evade them. [Magnetic Proxy documentation](https://www.magneticproxy.com/documentation) explains routing and restricted targets.

Magnetic Proxy is not affiliated with, endorsed by, or sponsored by Shopify. References to Shopify describe the third-party use case.

## Related resources and support

- [Magnetic Proxy product skill](https://github.com/MagneticProxy/magneticproxy-residential-proxy-agent-skills) for setup and product operation.
- [Magnetic Proxy Shopify use case](https://www.magneticproxy.com/use-cases/shopify-proxies?utm_source=github&utm_medium=agent_skill&utm_campaign=shopify-storefront-monitoring) for product context.
- [Report a reproducible issue](https://github.com/MagneticProxy/magneticproxy-shopify-storefront-monitoring-skill/issues) using redacted or synthetic examples. For account, billing or service issues, use support inside the product.
- [Contribution guide](CONTRIBUTING.md) and [security guidance](SECURITY.md).

This repository documents a specific task; it does not guarantee search rankings, AI citations, delivery, platform access or commercial results. Third-party names identify the workflow and do not imply endorsement.

## License

Original instructions and code are available under the [MIT License](LICENSE). Product subscriptions, service access and third-party data remain subject to their respective terms. This license does not grant trademark rights or permission to collect third-party content.
