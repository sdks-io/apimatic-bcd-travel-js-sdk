
# Reservation 9

*This model accepts additional fields of type unknown.*

## Structure

`Reservation9`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address` | [`Address5`](../../doc/models/address-5.md) | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `checkInDateTime` | `string` | Required | - |
| `checkOutDateTime` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `fare` | [`Fare2`](../../doc/models/fare-2.md) | Required | - |
| `guests` | [`Guest[]`](../../doc/models/guest.md) | Required | - |
| `lineItems` | `string[]` | Required | - |
| `numberOfNights` | `number` | Required | - |
| `numberOfRooms` | `number` | Required | - |
| `roomType` | `string` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `vendorChainCode` | `string` | Required | - |
| `vendorChainName` | `string` | Required | - |
| `vendorCode` | `string` | Required | - |
| `vendorName` | `string` | Required | - |
| `baseFare` | [`Fare \| undefined`](../../doc/models/fare.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address": {
    "address1": "Mahdentalstrasse 68.",
    "countryCode": "DE",
    "city": "Stuttgart",
    "postalCode": "71065",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "bookingDateTime": "bookingDateTime0",
  "checkInDateTime": "checkInDateTime4",
  "checkOutDateTime": "checkOutDateTime6",
  "confirmationNumber": "confirmationNumber6",
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
    "lineItems6",
    "lineItems7"
  ],
  "numberOfNights": 130,
  "numberOfRooms": 196,
  "roomType": "roomType2",
  "segmentNumber": 206,
  "vendorChainCode": "vendorChainCode2",
  "vendorChainName": "vendorChainName6",
  "vendorCode": "vendorCode8",
  "vendorName": "vendorName0",
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
```

