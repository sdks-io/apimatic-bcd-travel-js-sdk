
# Reservation 1

*This model accepts additional fields of type unknown.*

## Structure

`Reservation1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address` | [`Address1`](../../doc/models/address-1.md) | Required | - |
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
| `baseFare` | [`BaseFare1 \| undefined`](../../doc/models/base-fare-1.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address": {
    "address1": "Mahdentalstrasse 68.",
    "countryCode": "DE",
    "city": "Stuttgart",
    "postalCode": "71065",
    "region": "region2",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "bookingDateTime": "bookingDateTime8",
  "checkInDateTime": "checkInDateTime8",
  "checkOutDateTime": "checkOutDateTime4",
  "confirmationNumber": "confirmationNumber8",
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
    "lineItems8"
  ],
  "numberOfNights": 208,
  "numberOfRooms": 114,
  "roomType": "roomType0",
  "segmentNumber": 32,
  "vendorChainCode": "vendorChainCode0",
  "vendorChainName": "vendorChainName4",
  "vendorCode": "vendorCode0",
  "vendorName": "vendorName2",
  "baseFare": {
    "amount": 244.96,
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

