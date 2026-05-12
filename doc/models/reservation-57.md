
# Reservation 57

*This model accepts additional fields of type unknown.*

## Structure

`Reservation57`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address` | [`Address33`](../../doc/models/address-33.md) | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `checkInDateTime` | `string` | Required | - |
| `checkOutDateTime` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `fare` | [`Fare2`](../../doc/models/fare-2.md) | Required | - |
| `guests` | [`Guest[]`](../../doc/models/guest.md) | Required | - |
| `lineItems` | `string[]` | Required | - |
| `numberOfRooms` | `number` | Required | - |
| `roomType` | `string` | Required | - |
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
    "addressCountryCode": "DE",
    "addressLocality": "Stuttgart",
    "postalCode": "71065",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "bookingDateTime": "bookingDateTime2",
  "checkInDateTime": "checkInDateTime4",
  "checkOutDateTime": "checkOutDateTime2",
  "confirmationNumber": "confirmationNumber4",
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
    "lineItems4",
    "lineItems5",
    "lineItems6"
  ],
  "numberOfRooms": 240,
  "roomType": "roomType6",
  "vendorChainCode": "vendorChainCode6",
  "vendorChainName": "vendorChainName8",
  "vendorCode": "vendorCode6",
  "vendorName": "vendorName8",
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

