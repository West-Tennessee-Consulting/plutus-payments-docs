---
title: 'Adding Plutus Payments Invoice Generator Recipe'
description: 'Step-by-step guide on integrating Plutus Payments to generate invoices by clicking a button in a monday.com board'
keywords: 'Plutus Payments, monday.com, integration, invoicing, recipe, button click, Stripe, automation, documentation'
---

# How to Add Integration: Create an Invoice When Button is Clicked (with Mapped Values) in Board

This guide demonstrates how to set up a recipe to generate an invoice when a button is clicked. Screenshots and video clips are included to guide you through creating your first test invoice. 

**Note:** This guide tests Invoice 4 located in the "Upcoming" group.

## Step 1: Copying ColumnID Values for Later Integration

In the "Upcoming" group:
- Hover to the right of every column label.
- Select the three dots, then choose "ColumnID" to copy.

![ColumnID Copying](/img/when_buton_clicked_mapped/52.png)

In a note, paste the ColumnIDs for the following columns:
- Name (format: "FirstNameColumnID"SPLIT"LastNameColumnID")
- Address
- Phone
- Email
- City
- Zip
- State

These will be used later in the "Filling out the Remaining Fields" step.

## Step 2: Adding the Integration

1. Click the three dots menu on the top right of the board.
2. Select "Board Power-Ups" and then "Integrations".
3. Click on "Board Integrations" and then "+Add new integration".
4. In the Integrations Center, under "Explore by App", type "Stripe" and select the Stripe Invoice feature.
5. Choose "When button clicked Create an Invoice (w/Mapped) in Board with mapped values except for amount."

![Integration Configuration](../img/plutus/when_buton_clicked_mapped/When%20button%20clicked%20wmapped%20values%20screenshot%2045.png)

[Watch Video: Adding Integration - Part 1](https://youtu.be/BLMC4s3BG-E)

## Step 3: Connecting Stripe by Adding Secret Key

1. Copy the secret key from Stripe by navigating to [Stripe Dashboard](https://dashboard.stripe.com/dashboard).
2. Toggle Stripe into test mode and select "Developers" > "Reveal test key".
3. Copy the key starting with "sk_test_" and paste it into your recipe.

![Copying Secret Key](../img/plutus/when_buton_clicked_mapped/When%20button%20clicked%20wmapped%20screenshot%2050.png)

[Watch Video: Copying Secret Key - Part 2](https://www.youtube.com/watch?v=roijLB8hf78)

## Step 4: Filling out the Remaining Field Values

Paste the mapped ColumnIDs from your note into the "Invoice" settings.

![Filling Field Values](/img/when_buton_clicked_mapped/58.png)

Click "Done" and then "Add to Board".

[Watch Video: Filling Field Values - Part 3](https://www.youtube.com/watch?v=ZbnRcGtZBdo)

## Step 5: Testing Integration

To test the integration, select "Click Me" under the "Generate WTC Invoice" column in the "Upcoming" group.

![Testing Integration](/img/when_buton_clicked_mapped/61.png)

After clicking, an invoice will be generated, and a corresponding invoice link will appear in the group.

[Watch Video: Testing Integration - Part 4](https://www.youtube.com/watch?v=P-yBgAPWp-o)

Repeat these steps for any Stripe integration feature utilizing mapped field values.
