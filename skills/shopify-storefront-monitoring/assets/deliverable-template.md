# Shopify Price and Stock Monitoring with Magnetic Proxy deliverable

## Decision

State the actionable conclusion, the evidence supporting it and any condition that could change it.

## Scope and product operation

Record input owner, permitted purpose, source count, requested markets or audience, approved budget, account access state and execution timestamp. State whether the brand was actually operated or execution remains pending.

## Results

Complete `output.csv` using observed values. Use empty values plus explicit pending/unknown reasons when evidence is missing. Keep the source immutable and evidence private. Treat the file as an output contract, not a provider upload format. Escape spreadsheet formula prefixes in human-facing exports and preserve raw evidence separately.

## Exceptions and reconciliation

Account for every source record once, with a separate duplicate map where needed. Report missing, blocked, excluded and uncertain records without promoting them to success.

## Next action

Identify the owner, next reversible step and unresolved approval. Recommend a plan only for a measured capacity gap. Sending, scheduling, purchasing and changing external systems require their own authorization.

## Storefront change log

| Store and canonical URL | Product and variant | Displayed market and currency | Previous observation | Current observation | Evidence | Classification |
|---|---|---|---|---|---|---|
| Authorized target | Exact size/color/pack | Separate from exit country | Value and UTC timestamp | Value and UTC timestamp | Page excerpt or private screenshot | Confirmed change, unavailable or context mismatch |

## Merchandising decisions

Separate item addition/removal, displayed availability, item price and promotion changes. Missing from one collection is not removed from the catalog. Recheck material changes and identify which merchant decision they support.
