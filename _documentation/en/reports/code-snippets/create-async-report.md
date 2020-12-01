---
title: Create report
description: Creation of a report asynchronously.
navigation_weight: 3
---

# Create report asynchronously

This code snippet shows you how to generate a report asynchronously, using a date range.

This is an asynchronous call and so will return immediately. You can check the current status of report generation with [Get Report Status](/reports/code-snippets/get-report-status). Once completed, you can obtain the report with [Get Report](/reports/code-snippets/get-report). Alternatively, you can set a callback URL and receive a notification when report generation is complete.

Date range is limited to 13 months for this call.

## Example

```snippet_variables
- VONAGE_API_KEY
- VONAGE_API_SECRET
- ACCOUNT_ID.REPORTS
- REPORT_DIRECTION
- REPORT_PRODUCT
- REQUEST_ID.REPORTS
- DATE_START.REPORTS
- DATE_END.REPORTS
- STATUS.REPORTS
```

```code_snippets
source: '_examples/reports/create-async-report'
```

## Try it out

1. Set the replaceable variables for your account.  

2. For this example, set `REPORT_PRODUCT` to one of `SMS`, `VOICE` or `MESSAGES`.

3. Using the table as a guide set values for the remaining variables.

4. Run the script and you receive a response similar to the following:

```json
{
  "request_id": "ri3p58f-42d57cfd-1234-5678-9abc-67580d95f54a",
  "request_status": "PENDING",
  "direction": "outbound",
  "product": "SMS",
  "account_id": "abcd1234",
  "date_start": "2020-05-21T13:27:00+0000",
  "date_end": "2020-05-21T13:57:00+0000",
  "include_subaccounts": false,
  "include_message": false,
  "receive_time": "2020-06-04T10:53:32+0000",
  "_links": {
    "self": {
      "href": "https://api.nexmo.com/v2/reports/ri3p58f-42d57cfd-1234-5678-9abc-67580d95f54a"
    }
  }
}
```

If you set a callback URL, you will receive a callback on that URL with the same content as shown in the previous step.

## See also

* [Information on valid parameters](/reports/code-snippets/before-you-begin#parameters)
* [API Reference](/api/reports)
