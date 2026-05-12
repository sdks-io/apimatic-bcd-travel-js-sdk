
# Reservation 3

*This model accepts additional fields of type unknown.*

## Structure

`Reservation3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bookingDateTime` | `string` | Required | - |
| `carType` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `endDateTime` | `string` | Required | - |
| `endLocationAddress` | [`EndLocationAddress`](../../doc/models/end-location-address.md) | Required | - |
| `fare` | [`BaseFare`](../../doc/models/base-fare.md) | Required | - |
| `isInternational` | `boolean` | Required | - |
| `numberOfNights` | `number` | Required | - |
| `numberOfRooms` | `number` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `startDateTime` | `string` | Required | - |
| `startLocationAddress` | [`EndLocationAddress`](../../doc/models/end-location-address.md) | Required | - |
| `vendorChainName` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "bookingDateTime": "2022-02-11T09:19:00Z",
  "carType": "LIMO",
  "confirmationNumber": "5831",
  "endDateTime": "2022-03-01T08:00:00Z",
  "endLocationAddress": {
    "address1": "EWR AIRPORT UA 2310",
    "address2": "EWR AIRPORT UA 2511",
    "countryCode": "AE",
    "city": "Dubai",
    "postalCode": "779944",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "fare": {
    "amount": 2,
    "currencyCode": "USD",
    "description": "Estimated Total",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "isInternational": false,
  "numberOfNights": 14,
  "numberOfRooms": 1,
  "segmentNumber": 9,
  "startDateTime": "2022-02-15T09:45:00Z",
  "startLocationAddress": {
    "address1": "14 COPE CT HILLSBOROUGH",
    "address2": "27 NOPE ST WILLSBOROUGH",
    "countryCode": "CE",
    "city": "LHR",
    "postalCode": "555444",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "vendorChainName": "ADDISON",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

