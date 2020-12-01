---
title: Before you begin
navigation_weight: 1
---

# Before you Begin

## What are Code Snippets?

Code snippets are short pieces of code you can reuse in your own applications.
The code snippets use code from [example repositories](https://github.com/topics/nexmo-quickstart).

Please read this information carefully before attempting to use the code snippets.  

## Prerequisites

1. [Create a Vonage account](/account/guides/dashboard-management#create-and-configure-a-nexmo-account)
2. [Rent a Vonage Number](/numbers/guides/number-management#rent-a-virtual-number)
3. [Install the Vonage Library for your programming language](/tools)
4. [Set up Ngrok](https://ngrok.com)

## Other resources:

The following resources will help you use the [Number Insight Advanced Async](number-insight-advanced-async) code snippet:

- [Webhooks](/concepts/guides/webhooks)
- [Using Ngrok for local development](/tools/ngrok)

## Replaceable variables

Replace the following values in the code snippets with your own details:

```snippet_variables
- VONAGE_API_KEY
- VONAGE_API_SECRET
- INSIGHT_NUMBER
```

## Webhooks

The Basic and Standard levels of the Number Insight API are synchronous and do not require webhooks.

The Advanced level of the Number Insight API enables you to optionally deliver an asynchronous `POST` response to a webhook when the data becomes available.

In the code snippets, the webhook is located at `/webhooks/insight`. If you are using Ngrok, the webhook you need to configure in your client is of the form `https://demo.ngrok.io/webhooks/insight`. Replace `demo` with the subdomain provided by Ngrok.
