
# Ticket 1

*This model accepts additional fields of type unknown.*

## Structure

`Ticket1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `legs` | [`Leg2[]`](../../doc/models/leg-2.md) | Required | - |
| `recordLocator` | `string` | Required | - |
| `issueDateTime` | `string` | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `fare` | [`BaseFare1`](../../doc/models/base-fare-1.md) | Required | - |
| `payments` | `string[]` | Required | - |
| `lineItems` | `string[]` | Required | - |
| `passenger` | [`Passenger`](../../doc/models/passenger.md) | Required | - |
| `isInternational` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "legs": [
    {
      "arrivalDateTime": "2022-02-28T12:08:00Z",
      "arrivalStationCode": "ZWS",
      "carrierCode": "LH",
      "carrierName": "Lufthansa",
      "departureDateTime": "2022-02-28T10:52:00Z",
      "departureStationCode": "FRA",
      "segmentNumber": 3,
      "trainNumber": "3410",
      "classOfServiceCode": "classOfServiceCode8",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "recordLocator": "2CMDF7",
  "issueDateTime": "2022-01-06T17:03:00Z",
  "bookingDateTime": "2022-01-06T17:03:00Z",
  "fare": {
    "amount": 4574.77,
    "currencyCode": "USD",
    "description": "Total Fare",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "payments": [],
  "lineItems": [],
  "passenger": {
    "firstName": "FIRSTNAME",
    "lastName": "NONAME",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "isInternational": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

