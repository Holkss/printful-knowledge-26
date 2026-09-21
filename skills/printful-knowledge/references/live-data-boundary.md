# Live-data boundary

This skill works without a Printful API key.

## Knowledge is enough for

- explaining Printful terminology;
- explaining products vs variants;
- explaining production methods conceptually;
- explaining mockup/product/order/shipping workflows;
- interpreting public documentation;
- deciding what should be checked before a production or pricing decision.

## Current public verification may be needed for

- current prices;
- current product/variant availability;
- current regional availability;
- current shipping rates or estimates;
- current supported placements/techniques;
- current API endpoint/request/response behavior.

Use current official public Printful sources where available.

## Authenticated integration may be needed for

- the user's own store products or sync state;
- private file-library contents;
- account-specific discounts/settings;
- the user's orders and statuses;
- creating/editing/deleting/publishing account resources;
- placing or confirming orders;
- other account-scoped facts not available publicly.

## Credential rule

Never ask the user to paste a Printful API token into ordinary chat.

Credentials belong in a supported integration, secret store, environment configuration, or equivalent secure connection mechanism.

If no integration exists, explain the minimum connection needed instead of pretending the account was queried.
