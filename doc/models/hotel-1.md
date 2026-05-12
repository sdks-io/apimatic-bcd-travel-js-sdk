
# Hotel 1

*This model accepts additional fields of type unknown.*

## Structure

`Hotel1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `reservations` | [`Reservation6[]`](../../doc/models/reservation-6.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "c15d8f3d-9371-f61d-a300-39f66c60e7a0",
  "reservations": [
    {
      "address": {
        "address1": "47000 Lakeview Blvd",
        "countryCode": "US",
        "city": "Fremont",
        "region": "California",
        "postalCode": "94538",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "bookingDateTime": "2022-02-11T09:19:00Z",
      "checkInDateTime": "2022-02-15T15:00:00Z",
      "checkOutDateTime": "2022-03-01T11:00:00Z",
      "confirmationNumber": "91495930",
      "fare": {
        "amount": 1554,
        "currencyCode": "USD",
        "description": "Estimated Total",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "baseFare": {
        "amount": 78,
        "currencyCode": "USD",
        "description": "Daily",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "guests": [
        {
          "lastName": "DOE JOHN MR",
          "identifiers": [],
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "lineItems": [],
      "numberOfNights": 14,
      "numberOfRooms": 1,
      "roomType": "TED",
      "segmentNumber": 6,
      "vendorChainCode": "CY",
      "vendorChainName": "COURTYARD",
      "vendorCode": "17080",
      "vendorName": "Courtyard Fremont Marriott",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "address": {
        "address1": "304 E Cesar Chavez St",
        "countryCode": "US",
        "city": "Austin",
        "region": "Texas",
        "postalCode": "78701",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "bookingDateTime": "2022-02-11T09:19:00Z",
      "checkInDateTime": "2022-03-01T15:00:00Z",
      "checkOutDateTime": "2022-03-08T11:00:00Z",
      "confirmationNumber": "90736911",
      "guests": [
        {
          "lastName": "DOE JOHN MR",
          "identifiers": [],
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "lineItems": [],
      "numberOfNights": 7,
      "numberOfRooms": 1,
      "roomType": "TED",
      "segmentNumber": 7,
      "vendorChainCode": "MC",
      "vendorChainName": "MARRIOTT",
      "vendorCode": "385152",
      "vendorName": "Austin Marriott Downtown",
      "fare": {
        "amount": 128,
        "currencyCode": "currencyCode0",
        "description": "description0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "baseFare": {
        "amount": 242,
        "currencyCode": "currencyCode6",
        "description": "description4",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
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

