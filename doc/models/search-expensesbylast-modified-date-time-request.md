
# Search Expensesbylast Modified Date Time Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbylastModifiedDateTimeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter8`](../../doc/models/filter-8.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 10,
  "offset": 0,
  "filter": {
    "lastModifiedDateTime": "2022-02-11T21:12",
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

