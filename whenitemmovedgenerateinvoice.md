---
title: 'Adding Stripe Invoice Generator Integration for Item Movement in monday.com'
description: 'Step-by-step guide on integrating Stripe to automatically generate invoices when an item is moved to a specific group in monday.com'
keywords: 'Stripe, integration, invoice generator, monday.com, board integration, item movement, automation, documentation'
---

# Adding When an Item is Moved to a Group Integration for Stripe Invoice Generation

To test the integration, please input the following as a test invoice:

![Invoice Screenshot 1](/img/when_item_is_moved_to_group/Invoice%202%20Screenshot%2025.png)
![Invoice Screenshot 2](../img/plutus/when_item_is_moved_to_group/Invoice%202%20Screenshot%2026.png)
![Invoice Screenshot 3](../img/plutus/when_item_is_moved_to_group/Invoice%202%20Screenshot%2027.png)
![Invoice Screenshot 4](../img/plutus/when_item_is_moved_to_group/Invoice%202%20Screen%20Shot%2028.png)

In this guide, we demonstrate how to add a recipe to generate an invoice by moving an item into a board group. Screenshots and video clips are included to guide you through creating your first test invoice.

## Adding the Integration

1. Click the three dots menu on the top right of the board.
2. Select "Board Power-Ups" and then "Integrations".
3. Click on "Board Integrations" and then "+Add new integration".
4. In the Integrations Center, under "Explore by App", type "Stripe" and select the Stripe Invoice feature.
5. Choose "When an item is moved to group call the Stripe Invoice Generator to generate an Invoice".

![Integration Configuration](../img/plutus/when_item_is_moved_to_group/When%20an%20item%20is%20moved%20to%20group%20Screen%20Shot%2022.png)

The following recipe should be shown:

![Integration Recipe](../img/plutus/when_item_is_moved_to_group/When%20adding%20an%20Item%20Screen%20Shot%2023.png)

[Click to watch adding when item moved generate invoice integration feature](https://www.youtube.com/watch?v=VwTwQdDLCUI)

Select "Group" and choose "Pending Payment" for this integration. This way, any new invoices created in monday.com can be generated simply by changing the "Status" field in the "Upcoming" board.

![Select Group](../img/plutus/when_item_is_moved_to_group/When%20an%20Itme%20is%20moved%20screenshot%2024.png)
![Select Invoice](../img/plutus/when_item_is_moved_to_group/When%20an%20Item%20is%20Moved%20Screenshot%2025.png)

### Connecting Stripe by Adding Our Secret Key

Click "Invoice" in white. We want to first copy the secret key from Stripe.

To copy the secret key, open the [Stripe dashboard](https://dashboard.stripe.com/dashboard), toggle Stripe into test mode, select developers, and under "Standard Keys" choose "Reveal test key". Copy this key and paste it into our recipe. The test key will start with "sk_test_...".

[Click to watch video about copying secret key](https://www.youtube.com/watch?v=roijLB8hf78)

### Filling out the Remaining Fields

After the secret key is entered, please fill out the remaining fields.

[Click to watch video about copying Stripe secret key](https://www.youtube.com/watch?v=oEXTXeMRqQU)

![Invoice Fields 1](../img/plutus/when_item_is_moved_to_group/Adding%20Invoice%20Fields%20Screen%20Shot%2027.png)
![Invoice Fields 2](../img/plutus/when_item_is_moved_to_group/Adding%20Invoice%20Fields%20Screen%20Shot%2028.png)

Select "Done" and then "Add to Board" to save changes.

### Generate Invoice by Changing Status to Pending Test

To test the integration, change the status from "Upcoming" to "Invoice Pending Payment" in the "Upcoming" group.

![Generate Invoice Test](../img/plutus/when_item_is_moved_to_group/Generate%20Invoice%202%20Screen%20Shot%2029.png)

The invoice will automatically populate in the "Pending Payment" group with an invoice link.

![Generated Invoice](../img/plutus/when_item_is_moved_to_group/Generate%20Invoice%202%20Screen%20Shot%2030.png)
