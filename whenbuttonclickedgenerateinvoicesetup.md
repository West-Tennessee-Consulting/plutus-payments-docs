---
title: 'Adding Plutus Payments Invoice Generator Recipe'
description: 'Step-by-step guide on adding a recipe to generate invoices by clicking a button'
keywords: 'Plutus Payments, monday.com, integration, invoicing, recipe, button click, Stripe, automation, documentation'
---

# Stripe Integration - When Button is Clicked Generate an Invoice

# Adding Plutus Payments Invoice Generator Recipe to monday.com Board 

In this guide, we will show you how to add a recipe that enables the creation of an invoice by clicking a button. We'll provide screenshots and video clips to guide you through the process of generating your first test invoice.

We recommend using a board layout that divides invoices into three groups: Upcoming for invoices yet to be sent, Pending for sent invoices awaiting payment, and Completed for paid invoices.

## Introduction to Integration

We will demonstrate an integration that generates an invoice on Stripe.com. This integration is a critical step in the Plutus Payments application. After entering the necessary fields in the "Upcoming" monday.com board, users can generate an invoice by clicking the "Click Me" button.

![image](../img/plutus/1.png)

### Fill Out Necessary Fields for Testing

To test the integration, fill out a test invoice in the "Upcoming" board with the following information:

![image](/img/monday_sample_invoice_in_board/invoice_16.png)
![image](/img/plutus/monday_sample_invoice_in_board/invoice_17.png)
![image](../img/plutus/monday_sample_invoice_in_board/invoice_18.png)
![image](../img/plutus/monday_sample_invoice_in_board/invoice_19.png)
![image](../img/plutus/monday_sample_invoice_in_board/invoice_20.png)

### Adding the Integration

1. Click the three dots menu on the top right of the board.
2. Select "Board Power-Ups" and then "Integrations."
3. Click "Board Integrations" and then "+Add new integration."
4. Search for "Stripe" in the Integrations Center and select the Stripe Invoice Integration.
5. Choose the feature "When button clicked call the Stripe Invoice Generator to generate an Invoice" to open the recipe.

### Adding Button to the Integration

1. Click "Button" and select the "Generate Invoice" button column.

### Connecting Stripe by Adding Secret Key

1. Click "Invoice" and paste the secret key copied from the Stripe dashboard.
2. Make sure to fill out the remaining fields as shown in the video guide.

### Testing the Integration

Once the Integration is added, click "Click Me" to generate an invoice and test the integration.

If the Invoice Link field populates, the invoice generator works correctly. If not, double-check the secret key and seek support if needed.

For detailed steps, watch the provided video guides.

If you encounter any issues, please reach out to our support team for assistance.
