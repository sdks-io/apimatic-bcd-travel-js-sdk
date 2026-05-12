
# Search Expensesbyinvoice Date Timerange Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyinvoiceDateTimerangeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter6`](../../doc/models/filter-6.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 1,
  "offset": 1,
  "filter": {
    "invoiceDateTime": "2022-01-01T00:01 TO 2022-02-17T00:01",
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

