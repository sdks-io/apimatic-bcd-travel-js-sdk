
# Ticket 3

*This model accepts additional fields of type unknown.*

## Structure

`Ticket3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `legs` | [`Leg4[]`](../../doc/models/leg-4.md) | Required | - |
| `recordLocator` | `string` | Required | - |
| `issueDateTime` | `string` | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `fare` | [`Fare`](../../doc/models/fare.md) | Required | - |
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
      "arrivalDateTime": "2022-03-09T10:06:00Z",
      "arrivalStationCode": "QDU",
      "carrierCode": "LH",
      "carrierName": "Lufthansa",
      "classOfServiceCode": "S",
      "departureDateTime": "2022-03-09T08:42:00Z",
      "departureStationCode": "FRA",
      "segmentNumber": 13,
      "trainNumber": "3502",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "recordLocator": "U7EKXS",
  "issueDateTime": "2022-02-11T09:19:00Z",
  "bookingDateTime": "2022-02-11T09:19:00Z",
  "fare": {
    "amount": 942.07,
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
    "firstName": "JOHN",
    "lastName": "DOE",
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

