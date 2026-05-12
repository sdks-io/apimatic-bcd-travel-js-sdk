
# Document

*This model accepts additional fields of type unknown.*

## Structure

`Document`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `documentNumber` | `string` | Required | - |
| `bookingType` | `string` | Required | - |
| `fare` | [`Fare`](../../doc/models/fare.md) | Required | - |
| `baseFare` | [`Fare`](../../doc/models/fare.md) | Required | - |
| `lineItems` | [`DocumentLineItems[]`](../../doc/models/containers/document-line-items.md) | Required | This is Array of a container for one-of cases. |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
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
```

