
# Car 16

*This model accepts additional fields of type unknown.*

## Structure

`Car16`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `reservations` | [`Reservation56[]`](../../doc/models/reservation-56.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "reservations": [
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

