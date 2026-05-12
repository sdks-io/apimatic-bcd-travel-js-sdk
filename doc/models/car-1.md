
# Car 1

*This model accepts additional fields of type unknown.*

## Structure

`Car1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `reservations` | [`Reservation4[]`](../../doc/models/reservation-4.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "e5b0a390-5913-5a87-0d11-b6e148ca2da3",
  "reservations": [
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
    },
    {
      "bookingDateTime": "2022-02-11T09:19:00Z",
      "carType": "Intermediate Car Auto A/C",
      "confirmationNumber": "K0350953567",
      "dropOffLocation": {
        "address1": "Austin Bergstrom Intl Airport",
        "address2": "3819 Presidential Blvd",
        "countryCode": "US",
        "city": "Austin",
        "region": "Texas",
        "postalCode": "78719-2339",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "endDateTime": "2022-03-08T10:00:00Z",
      "isInternational": false,
      "lineItems": [],
      "numberOfCars": 1,
      "pickupLocation": {
        "address1": "Austin Bergstrom Intl Airport",
        "address2": "3819 Presidential Blvd",
        "countryCode": "US",
        "city": "Austin",
        "region": "Texas",
        "postalCode": "78719-2339",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "rentalDays": 7,
      "segmentNumber": 10,
      "startDateTime": "2022-03-01T18:45:00Z",
      "vendorChainCode": "ZE",
      "vendorChainName": "Hertz Rent-A-Car",
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

