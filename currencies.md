---
title: 'Supported Currencies'
description: 'Learn about the supported currencies in Plutus Payments integration with Stripe and how to handle different payment currencies.'
keywords: 'Plutus Payments,wtc,memphis,tennessee,stripe,and,more,collection,methods,support,documentation'
---

# Supported Currencies

## Supported Currencies in Plutus Payments Integration with Stripe

Our current integration supports Stripe. Our team is in the process of developing support for more platforms. 

### Supported Currencies in Stripe

Our Stripe API integration supports over 135 different currencies. 

The currency defaults to that of the customer unless otherwise specified.

### Viewing Transaction Currency

To view the set currency of any transaction, please follow these steps:

1. Select the payments tab. 
2. Choose any succeeded transaction.
3. After opening the transaction, scroll down to "Events and Logs".
4. On the right, locate "invoice.payment_succeeded".
5. Finally, on row 8, you will see "currency": "***", as a three-letter ISO code. 

### Additional Information 

For information about setting or changing currencies, please follow the link below: 

[**Additional Information**](https://support.stripe.com/questions/set-or-change-currency-for-an-invoice-or-customer-in-stripe-billing)

### Handling Different Payment Currencies

Note: If the payer's currency differs from the charge currency, credit card companies may charge added exchange fees to customers. 

For more information, please click [here](https://stripe.com/docs/currencies).

### Setting One-Off Invoice Currency 

For more information about setting a default currency for one-off invoices, please click [here](https://support.stripe.com/questions/setting-a-customers-default-currency)
