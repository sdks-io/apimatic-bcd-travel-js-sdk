
# Search Expensesbycustomer Number Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbycustomerNumberRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter12`](../../doc/models/filter-12.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 10,
  "offset": 0,
  "filter": {
    "customerNumber": [
      "9999999999"
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

