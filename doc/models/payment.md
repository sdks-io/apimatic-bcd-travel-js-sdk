
# Payment

*This model accepts additional fields of type unknown.*

## Structure

`Payment`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productId` | `string` | Required | - |
| `amount` | `number \| undefined` | Optional | - |
| `paymentType` | `string` | Required | - |
| `currencyCode` | `string \| undefined` | Optional | - |
| `cardDetail` | [`CardDetail \| undefined`](../../doc/models/card-detail.md) | Optional | - |
| `authorizationCode` | `string \| undefined` | Optional | - |
| `ticketNumber` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "productId": "5b25731f-b4b9-d5e3-e076-381257310431",
  "amount": 5176.57,
  "paymentType": "Credit Card",
  "currencyCode": "USD",
  "cardDetail": {
    "type": "VI",
    "number": "9484",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "authorizationCode": "004511",
  "ticketNumber": "ticketNumber0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

