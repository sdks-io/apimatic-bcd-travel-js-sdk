
# Misc 10

*This model accepts additional fields of type unknown.*

## Structure

`Misc10`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `documents` | [`Document[]`](../../doc/models/document.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "documents": [
    {
      "documentNumber": "8904804804804",
      "bookingType": "Purchase",
      "fare": {
        "amount": 10.77,
        "currencyCode": "USD",
        "description": "Total Fare",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "baseFare": {
        "amount": 10.77,
        "currencyCode": "USD",
        "description": "Base Fare",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "lineItems": [],
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

