---
title: 'Plutus Payments Integration Setup Guide'
description: 'A comprehensive guide on integrating Plutus Payments with monday.com for efficient invoicing'
keywords: 'Plutus Payments, monday.com, integration, invoicing, setup guide, Stripe, automation, collection methods, documentation'
---

# Plutus Payments monday.com Application Set Up Guide

In this page, we will discuss the steps required to successfully integrate several key features from the Plutus Payments App on your monday.com board. Videos you may wish to follow will be provided as well. 

## Plutus Payments Demo Board Layout 

The board in this demo contains three groups:
1. **Upcoming:** Lists all upcoming invoices your firm wishes to charge.
2. **Pending Payment:** Lists all invoices that have been created and are waiting payment.
3. **Done:** Lists all invoices that have been paid successfully.

### The Following Setup Guides demonstrate how to add and test key Plutus Payment Integrations between monday.com and Stripe

We recommend this board layout which simply divides invoices into three different groups:
- **Upcoming:** For invoices that have yet to be sent.
- **Pending:** For sent invoices awaiting payment.
- **Completed:** For invoices that have been paid.

We will demonstrate an integration that generates an invoice on Stripe.com. This is a critical step of the Plutus Payments application. When successfully integrated, after the desired fields are entered in the "Upcoming" monday.com board, a user can select the "Click Me" button to generate an invoice.

![Plutus Payments Demo](/img/1.png)

### Fill Out Necessary Fields to Test the Integration

To test our integration, please fill out a test invoice in the "Upcoming" board. In this example, we used the following information:

![Test Invoice Fields](/img/monday_sample_invoice_in_board/invoice_16.png)
![Test Invoice Fields](/img/monday_sample_invoice_in_board/invoice_17.png)
![Test Invoice Fields](/img/monday_sample_invoice_in_board/invoice_18.png)
![Test Invoice Fields](/img/monday_sample_invoice_in_board/invoice_19.png)
![Test Invoice Fields](/img/monday_sample_invoice_in_board/invoice_20.png)

### Adding the Integration

1. Select the three dots menu on the top right of the board.
2. Click on "Board Power-Ups" > "Integrations" > "Board Integrations".
3. Click "+Add new integration" > "Stripe Invoice Generator to generate an Invoice".
4. Connect Stripe by adding your secret key.
5. Fill out the remaining fields and click "Add To Board" to save the changes.

### Testing the Invoice Generator Integration

Now that the integration has been added, let's select "Click Me" and generate an invoice. If you see the Invoice Link field populate, then the invoice generator works correctly. If not, please ensure the secret key has been copied correctly.

## Adding Integration When an Item is Moved to a Group

To test the integration, input the following as a test invoice and change the status from "Upcoming" to "Invoice Pending Payment" in the "Upcoming" group.

![Test Invoice Fields](/img/when_item_is_moved_to_group/Invoice%202%20Screenshot%2025.png)
![Test Invoice Fields](/img/when_item_is_moved_to_group/Invoice%202%20Screenshot%2026.png)
![Test Invoice Fields](/img/when_item_is_moved_to_group/Invoice%202%20Screenshot%2027.png)
![Test Invoice Fields](/img/when_item_is_moved_to_group/Invoice%202%20Screen%20Shot%2028.png)

## Add Integration When Invoice Column Changes to Done

Invoices in the "Upcoming" group can be marked as done, working on it, or stuck. Any invoice marked as done should be automatically sent to the "Pending Payments" group and generated automatically.

## Add Integration When Button Clicked Create an Invoice (w/Mapped) in Board with Mapped Values Except for Amount

In this example, we are going to test "Invoice 4" located in the "Upcoming" group.

![Test Invoice Fields](/img/when_buton_clicked_mapped/53.png)
![Test Invoice Fields](/img/plutus/when_buton_clicked_mapped/54.png)
![Test Invoice Fields](/img/plutus/when_buton_clicked_mapped/55.png)

Please follow the steps outlined in the documentation to set up and test each integration.
