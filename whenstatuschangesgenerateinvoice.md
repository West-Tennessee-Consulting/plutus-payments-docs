---
title: 'Automate Invoice Generation on Status Change with Stripe Integration'
description: 'Learn how to automatically generate invoices in monday.com when the status of an invoice changes using the "When status changes to something call the Stripe Invoice Generator to Generate an Invoice" feature.'
keywords: 'monday.com, integration, invoicing, automation, invoice generation, status change, Stripe, documentation'
---

# Add When Invoice Column Changes to Done Generate an Invoice

Invoices in the "Upcoming" group can be marked as done, working on it, or stuck.
    
Any invoice marked as done should be automatically sent to the Pending Payments group and generate automatically. 

In order for this to occur, we will add the "When status changes to something call the Stripe Invoice Generator to generate an Invoice" feature. 

In this example we have a test invoice in the "Upcoming" group labelled "Test Invoice 3".

![image](../img/plutus/when_status_changes_generate_an_invoice/31.png)

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2032.png)

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20Status%20Changes%20Screen%20shot%2033.png)

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2034.png)


Using the example above, we are going to show how to add a recipe which grants the creation of an invoice.

We will provide screenshots and video clips along the way to help guide you to make your first test invoice.

### Adding the Integration

Next select the three dots menu on the top right of the board. 
This will show a list of board permissions, settings, and notifications. 

![image](../img/plutus/1.2.png)    

Click on "Board Power-Ups" 
You will see Board Views, Dashboards, Integrations and Automations. 

![image](../img/plutus/3.png)

Please select Integrations. 

![image](../img/plutus/4.png) 

You will see three tabs which are Integrations Center, Board Integrations, Account Usage. 
Select Board Integrations. 
On the top right select "+Add new integration".

![image](../img/plutus/5.png)

This will open the Integrations Center.
 
![image](../img/plutus/6.png)

Under the Category "Explore by App" type Stripe.

![image](../img/plutus/7.png)  

Please Select the Stripe Invoice Feature. 

Once the integration is opened a list of features will be shown. 

We want to select the feature called "When status changes to something call the Stripe Invoice Generator to Generate an Invoice". 

[**Click to watch video about opening Stripe integration feature list**](https://www.youtube.com/watch?v=BUdPK-t4VWM)
 
![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2035.png)

We will edit invoice, something, and status. 

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2036.png)
 
Open "status" and then select invoice. 

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2037.png)

Open "something" and then select done.

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2038.png)

Open "Invoice".

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2039.png)

[**Click to watch video about editing Stripe Invoice Generator**](https://www.youtube.com/watch?v=h2pejE2hk4g)

### Connecting Stripe by Adding our Secret Key

We want to first copy the secret key from Stripe. 

To copy the secret key. 

Open the Stripe dashboard from the link below. 

[Link](https://dashboard.stripe.com/dashboard) 

![image](../img/plutus/11.png)

Toggle Stripe into test mode using the switch located on the top right. 

![image](../img/plutus/12.png)

Next to test mode select developers. 
Under "Standard Keys" select "Reveal test key".
Copy this key and paste into our recipe. 
The test key will start with "sk_test_...".

Please note that we are using a secret key in test mode to test an invoice. 
Later we will have to close test mode and then copy the actual secret key into our recipe. 

![image](../img/plutus/13.png) 

[**Click to watch video about copying Stripe secret key**](https://www.youtube.com/watch?v=roijLB8hf78)

### Filling out the Remaining Fields

After the secret key is entered please fill out the remaining fields from Test Invoice 3. 

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20status%20changes%20screen%20shot%2040.png)

![image](../img/plutus/when_status_changes_generate_an_invoice/When%20
