# Stores, products, and orders

## Store context

Printful product-management behavior can differ by store/integration type.

Do not assume an endpoint or workflow for a Manual/API store necessarily creates or edits products on an external ecommerce platform.

## Product configuration

Exact product configuration can require:
- the relevant catalog variant;
- production files;
- placement/technique information;
- store/product context.

Never infer missing IDs or silently substitute a Product ID for a Variant ID.

## Orders

Explain the difference between estimating/drafting an order and submitting/confirming an order.

If an authenticated integration exists:
- default to read-only work for fact finding;
- require explicit user intent for writes;
- obtain fresh explicit confirmation immediately before an action that can spend money, start fulfillment, delete data, or publish a consequential customer-visible change.
