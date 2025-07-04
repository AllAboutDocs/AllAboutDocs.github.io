## List Docs contents and expiring contents by Docs ID

This request retrieves the current Docs contents and other contents that will expire soon for a specific Docs ID. The details can be retrieved using the following:

### Query parameters - Required\*

- `id` - the unique internal identifier for the Docs
- `Docs-Entity-ID` - the unique identifier of the third party entity

The retrieved response displays the details associated with the specified Docs ID.

**URL**

`{URL}/v1/docs/{id}/contents`

**METHOD**

GET

**SUCCESS RESPONSE**

200: The Docs contents details are displayed.

**SAMPLE RESPONSE**

```JSON
{
  "id": "0f5w7ir5wcqj8ydeih3wpv0807",
  "aggregatedcontents": {
    "primary": {
      "type": "SAR",
      "value": 5
    }
  },
  "accounts": [
    {
      "accountType": "string",
      "contents": {
        "type": "SAR",
        "value": 5
      },
      "expiringcontents": [
        {
          "amount": {
            "type": "SAR",
            "value": 5
          },
          "expirationDateTime": "2023-12-12T10:16:38Z"
        }
      ]
    }
  ]
}
```
