
# Filter

*This model accepts additional fields of type unknown.*

## Structure

`Filter`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `invoiceNumber` | `string[]` | Required | - |
| `travelerEmail` | `string[]` | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `invoiceDateTime` | `string` | Required | - |
| `lastModifiedDateTime` | `string` | Required | - |
| `customerNumber` | `string[]` | Required | - |
| `accountId` | `string[]` | Required | - |
| `globalCustomerNumber` | `string[]` | Required | - |
| `hasTransaction` | `boolean` | Required | - |
| `recordLocator` | `string[]` | Required | - |
| `ticketStatus` | `string[]` | Required | - |
| `calculatedTicketStatus` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "invoiceNumber": [
    "850176",
    "850177"
  ],
  "travelerEmail": [
    "FIRSTNAME.NONAME@COMPANY.COM",
    "JDOE@SOMEWHERE.COM"
  ],
  "bookingDateTime": "2022-01-01T00:01 TO 2022-02-17T00:01",
  "invoiceDateTime": "2022-01-01T00:01 TO 2022-02-17T00:01",
  "lastModifiedDateTime": "2022-01-01T00:01 TO 2022-02-17T00:01",
  "customerNumber": [
    "9999999999",
    "9999999"
  ],
  "accountId": [
    "999999901",
    "999999902"
  ],
  "globalCustomerNumber": [
    "9999",
    "20109999"
  ],
  "hasTransaction": true,
  "recordLocator": [
    "GKQLV1",
    "EKDCAG"
  ],
  "ticketStatus": [
    "TICKETED"
  ],
  "calculatedTicketStatus": [
    "USED/FLOWN"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

