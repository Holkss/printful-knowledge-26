# Core concepts

## Catalog Product

A Catalog Product is the product/model grouping in Printful's catalog.

## Catalog Variant

A Catalog Variant is a specific physical variation of a Catalog Product, commonly a size/color combination and sometimes another distinguishing attribute.

## Product ID vs Variant ID

A Product ID identifies the product grouping. A Variant ID identifies an exact variant.

Do not substitute one for the other. When an operation targets an exact physical item, verify whether the current Printful contract expects a variant identifier.

## Sync Product and Sync Variant

For connected ecommerce stores, Printful uses synchronized product concepts that represent store-side products and variants and their relationship to Printful production configuration.

Do not assume Catalog Product, Catalog Variant, Sync Product, and Sync Variant are interchangeable.

## Product template

A product template is a reusable configuration concept. Keep it distinct from store-synced product objects unless current official documentation explicitly connects them for the requested operation.

## Knowledge vs current fact

Conceptual relationships are relatively stable. Availability, prices, shipping, fulfillment, supported placements/techniques, and API behavior can change and should be treated as current facts when a decision depends on them.
