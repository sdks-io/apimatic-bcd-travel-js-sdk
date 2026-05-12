
# Reservation 6

*This model accepts additional fields of type unknown.*

## Structure

`Reservation6`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address` | [`Address3`](../../doc/models/address-3.md) | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `checkInDateTime` | `string` | Required | - |
| `checkOutDateTime` | `string` | Required | - |
| `confirmationNumber` | `string` | Required | - |
| `fare` | [`BaseFare \| undefined`](../../doc/models/base-fare.md) | Optional | - |
| `baseFare` | [`BaseFare \| undefined`](../../doc/models/base-fare.md) | Optional | - |
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
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
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
}
```

