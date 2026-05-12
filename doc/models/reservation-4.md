
# Reservation 4

*This model accepts additional fields of type unknown.*

## Structure

`Reservation4`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `bookingDateTime` | `string` | Required | - |
| `carType` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `dropOffLocation` | [`DropOffLocation1`](../../doc/models/drop-off-location-1.md) | Required | - |
| `endDateTime` | `string` | Required | - |
| `isInternational` | `boolean` | Required | - |
| `lineItems` | `string[]` | Required | - |
| `numberOfCars` | `number` | Required | - |
| `pickupLocation` | [`DropOffLocation1`](../../doc/models/drop-off-location-1.md) | Required | - |
| `rentalDays` | `number` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `startDateTime` | `string` | Required | - |
| `vendorChainCode` | `string` | Required | - |
| `vendorChainName` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "bookingDateTime": "2022-02-11T09:19:00Z",
  "carType": "Intermediate Car Auto A/C",
  "confirmationNumber": "K03512717C2",
  "dropOffLocation": {
    "address1": "Hertz San Francisco International Airport",
    "address2": "780 McDonnell Road",
    "countryCode": "US",
    "city": "San Francisco",
    "region": "California",
    "postalCode": "94128",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "endDateTime": "2022-03-01T11:00:00Z",
  "isInternational": false,
  "lineItems": [],
  "numberOfCars": 1,
  "pickupLocation": {
    "address1": "Hertz San Francisco International Airport",
    "address2": "780 McDonnell Road",
    "countryCode": "US",
    "city": "San Francisco",
    "region": "California",
    "postalCode": "94128",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "rentalDays": 13,
  "segmentNumber": 5,
  "startDateTime": "2022-02-16T17:00:00Z",
  "vendorChainCode": "ZE",
  "vendorChainName": "Hertz Rent-A-Car",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

