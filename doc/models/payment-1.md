
# Payment 1

*This model accepts additional fields of type unknown.*

## Structure

`Payment1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
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
  "ticketNumber": "ticketNumber4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

