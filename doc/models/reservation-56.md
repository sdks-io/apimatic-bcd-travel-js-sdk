
# Reservation 56

*This model accepts additional fields of type unknown.*

## Structure

`Reservation56`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bookingDateTime` | `string` | Required | - |
| `carType` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `dropOffLocation` | [`DropOffLocation16`](../../doc/models/drop-off-location-16.md) | Required | - |
| `endDateTime` | `string` | Required | - |
| `fare` | [`Fare`](../../doc/models/fare.md) | Required | - |
| `baseFare` | [`BaseFare`](../../doc/models/base-fare.md) | Required | - |
| `isInternational` | `boolean` | Required | - |
| `lineItems` | `string[]` | Required | - |
| `numberOfCars` | `number` | Required | - |
| `pickupLocation` | [`DropOffLocation16`](../../doc/models/drop-off-location-16.md) | Required | - |
| `rentalDays` | `number` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `startDateTime` | `string` | Required | - |
| `vendorChainCode` | `string` | Required | - |
| `vendorChainName` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "bookingDateTime": "2022-01-06T17:03:00Z",
  "carType": "Compact 4DR Car Manual AC",
  "confirmationNumber": "9917132564",
  "dropOffLocation": {
    "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
    "addressCountryCode": "DE",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "endDateTime": "2022-03-03T17:00:00Z",
  "fare": {
    "amount": 400.95,
    "currencyCode": "EUR",
    "description": "Estimated Total",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "baseFare": {
    "amount": 100,
    "currencyCode": "EUR",
    "description": "Daily",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "isInternational": false,
  "lineItems": [],
  "numberOfCars": 1,
  "pickupLocation": {
    "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
    "addressCountryCode": "DE",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "rentalDays": 4,
  "segmentNumber": 5,
  "startDateTime": "2022-02-28T12:00:00Z",
  "vendorChainCode": "SX",
  "vendorChainName": "Sixt Rent a Car",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

