
# Search Expenses Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter`](../../doc/models/filter.md) | Required | - |
| `sort` | [`Sort`](../../doc/models/sort.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 50,
  "offset": 0,
  "filter": {
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
  },
  "sort": {
    "lastModifiedDateTime": "asc",
    "invoiceDateTime": "desc",
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

