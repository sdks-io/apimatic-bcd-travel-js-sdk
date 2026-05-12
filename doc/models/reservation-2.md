
# Reservation 2

*This model accepts additional fields of type unknown.*

## Structure

`Reservation2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bookingDateTime` | `string` | Required | - |
| `cabin` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `endDateTime` | `string` | Required | - |
| `fare` | [`BaseFare`](../../doc/models/base-fare.md) | Required | - |
| `linkCode` | `string` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `shipName` | `string` | Required | - |
| `startDateTime` | `string` | Required | - |
| `vendorChainCode` | `string` | Required | - |
| `vendorChainName` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "bookingDateTime": "2022-02-11T09:19:00Z",
  "cabin": "TURISTAFLEXIBLE",
  "confirmationNumber": "4561",
  "endDateTime": "2022-03-01T08:00:00Z",
  "fare": {
    "amount": 802,
    "currencyCode": "USD",
    "description": "Estimated Total",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "linkCode": "A",
  "segmentNumber": 10,
  "shipName": "Angelena",
  "startDateTime": "2022-02-15T09:45:00Z",
  "vendorChainCode": "repudiandae",
  "vendorChainName": "erat",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

