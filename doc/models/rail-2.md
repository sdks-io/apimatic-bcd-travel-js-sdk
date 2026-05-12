
# Rail 2

*This model accepts additional fields of type unknown.*

## Structure

`Rail2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `tickets` | [`Ticket5[]`](../../doc/models/ticket-5.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "id2",
  "tickets": [
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

