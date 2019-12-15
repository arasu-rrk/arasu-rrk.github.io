---
title: How to send an SMTP mail using SendGrid?
author: arasu_rrk
show_comments: true
permalink: "/blog/how-to-send-an-smtp-mail-using-sendgrid"
categories: [ SendGrid, SMTP ]
image: assets/logos/sendgrid.jpg
tags: [sendgrid, smtp, csharp]
---

[SendGrid](https://sendgrid.com) (now owned by [Twilio](https://www.twilio.com)) is used by some of the biggest names in the industry such as Uber, Spotify, Yelp, Airbnb, and even Kinsta. It originally started out as a transactional email SMTP and API serviced designed for developers. However, they now also offer email marketing features as well.

1. Go to <https://app.sendgrid.com/settings/api_keys>
   ![](/images/sendgrid/sendgrid-api-keys-link.png)

2. Click the **Create API Key**.
   ![](/images/sendgrid/sendgrid-create-api-keys.png)

3. From the dialog select **Restricted Access**
   ![](/images/sendgrid/sendgrid-api-keys-options.png)

4. Enable the option **Mail Send -> Mail Send**
   ![](/images/sendgrid/sendgrid-api-keys-mail.png)

5. Once the API keys generated, please keep them in a safe place. You can't get the same key again and you need to regenerate a new key.
   ![](/images/sendgrid/sendgrid-api-keys-success.png)

6. Please use the following SMTP configuration in your application.

| Host     	| smtp.sendgrid.net                    	|
| Port     	| 587 or 465(SSL)                      	|
| Username 	| apikey (Yes. **apikey** is the username for all accounts)|
| Password 	| API key generated in the above steps 	|


## Code Sample

Please find the sample C# application in the below link.

<https://github.com/arasu-rrk/sendgrid-smtp-client>

<style>
  table, td {
    border: 1px solid black;
  }

  td{
    padding: 0 10px;
  }
</style>