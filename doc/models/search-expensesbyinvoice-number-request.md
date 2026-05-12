
# Search Expensesbyinvoice Number Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyinvoiceNumberRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter2`](../../doc/models/filter-2.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 10,
  "offset": 0,
  "filter": {
    "invoiceNumber": [
      "844680"
    ],
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

