# Prices Entered With Tax

This option is perhaps the most important when managing taxes in your store, as it determines how you input product prices later on.

* **“Yes, I will enter prices inclusive of tax”** means that all catalog prices are input using your store’s base tax rate.

For example, in the UK you would input prices inclusive of the 20% tax rate e.g. You enter a product price of £9.99 that includes £1.67 tax. A customer in the UK would pay £9.99 as defined, and a customer in the US would only pay £8.32.

* **“No, I will enter prices exclusive of tax”** would mean that your catalog prices need to be tax exclusive.

Using the example from above, a UK shop would enter 8.32 at the product price. A tax of 20% would be applied on top of this during checkout making the amount payable £9.99.

#### The tax calculation for tax-**inclusive** prices is:

`tax_amount = price - ( price / ( ( tax_rate_% / 100 ) + 1 ) )`

#### The tax calculation for tax-**exclusive** prices is:

`tax_amount = price * ( tax_rate_% / 100 )`

{% hint style="info" %}
More at: [How Taxes Work in WooCommerce.](https://github.com/woocommerce/woocommerce/wiki/How-Taxes-Work-in-WooCommerce)
{% endhint %}

