# Neuralis AI Identity Manager


Neuralis AI Identity Manager is a WordPress plugin for Generative Engine Optimization (GEO). Define your organization, people, services and products as reusable entities, then connect them to the pages that describe them. Neuralis publishes those relationships as Schema.org JSON-LD and a site knowledge graph.


**[Install the free plugin on WordPress.org](https://wordpress.org/plugins/neuralis-ai-identity-manager/)** · [Documentation and product site](https://aim.verri.pro/)


![Neuralis AI Identity Manager interface in WordPress showing entity management and knowledge graph features](https://aim.verri.pro/wp-content/uploads/2026/03/AI-Identity-Manager-Generative-Engine-Optimization-WordPress-plugin-1024x683.png)


## What Neuralis does


- Create entities once and reuse them across relevant WordPress pages.
- Set the primary subject of a page and add secondary entities where relevant.
- Generate JSON-LD, a connected knowledge graph and an `llms.txt` file.
- Inspect existing JSON-LD and manage overlaps with supported plugins using Schema Control.


## Example: connect a service to its provider


Create the provider as an organization and select it on the service entity. The service references the provider by its stable `@id`. Another service from the same organization can reference the same provider ID.


The excerpt below comes from a Neuralis test installation. It shows only the fields relevant to the relationship and uses `example.com` in place of the test hostname.


```json
{
  "@context": "https://schema.org",
  "@type": "Service",
  "@id": "https://example.com/aim-kg/service/12",
  "name": "Web Design",
  "provider": {
    "@id": "https://example.com/aim-kg/organization/1",
    "@type": "Organization"
  }
}
```


[Follow the WordPress setup guide and check the published JSON-LD](https://aim.verri.pro/docs/how-to-connect-a-service-page-to-its-provider-in-wordpress/).


## WooCommerce add-on

[Neuralis for WooCommerce](https://aim.verri.pro/neuralis-for-woocommerce/) automatically creates and synchronizes product, variation and approved customer review entities in the Neuralis Knowledge Graph.

- Create entities from published simple and variable WooCommerce products.
- Connect a ProductGroup to its individual Product variations and applicable offers.
- Keep product information, prices, stock availability and approved native reviews synchronized.

**Requirements:** WooCommerce, Neuralis Pro 1.2.0 or later with Pro functionality enabled, and a separate activated add-on license.

**License:** $50 one-time payment for one site, plus applicable taxes. Neuralis Pro is sold separately.

[Read the add-on overview](addons/neuralis-for-woocommerce.md) · [View the product page](https://aim.verri.pro/neuralis-for-woocommerce/)

## About


Developed by [Alessandro Verri](https://verri.pro/), marketing and Generative Engine Optimization consultant for small businesses.

