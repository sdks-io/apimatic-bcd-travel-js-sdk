
# Hotel 16

*This model accepts additional fields of type unknown.*

## Structure

`Hotel16`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `reservations` | [`Reservation57[]`](../../doc/models/reservation-57.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "reservations": [
    {
      "address": {
        "address1": "Mahdentalstrasse 68.",
        "addressCountryCode": "DE",
        "addressLocality": "Stuttgart",
        "postalCode": "71065",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "bookingDateTime": "bookingDateTime6",
      "checkInDateTime": "checkInDateTime0",
      "checkOutDateTime": "checkOutDateTime2",
      "confirmationNumber": "confirmationNumber0",
      "fare": {
        "amount": 50,
        "currencyCode": "currencyCode0",
        "description": "description0",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "guests": [
        {
          "lastName": "NONAME FIRSTNAME",
          "identifiers": [],
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "lineItems": [
        "lineItems0",
        "lineItems1"
      ],
      "numberOfRooms": 248,
      "roomType": "roomType8",
      "vendorChainCode": "vendorChainCode8",
      "vendorChainName": "vendorChainName2",
      "vendorCode": "vendorCode2",
      "vendorName": "vendorName4",
      "baseFare": {
        "amount": 2.42,
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

