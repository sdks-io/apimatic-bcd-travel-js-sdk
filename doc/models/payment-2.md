
# Payment 2

*This model accepts additional fields of type unknown.*

## Structure

`Payment2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productId` | `string` | Required | - |
| `amount` | `number` | Required | - |
| `paymentType` | `string` | Required | - |
| `currencyCode` | `string` | Required | - |
| `cardDetail` | [`CardDetail`](../../doc/models/card-detail.md) | Required | - |
| `authorizationCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "productId": "1cc25604-13ef-0b36-3d5e-948f4a01e00d",
  "amount": 942.07,
  "paymentType": "Credit Card",
  "currencyCode": "EUR",
  "cardDetail": {
    "type": "CA",
    "number": "1234",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "authorizationCode": "01010 C",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

