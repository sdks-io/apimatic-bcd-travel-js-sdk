
# Search Expensesbylast Modified Date Timerange Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbylastModifiedDateTimerangeRequest`

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
  "limit": 1,
  "offset": 1,
  "filter": {
    "lastModifiedDateTime": "2022-02-01T21:12 TO 2022-02-17T10:40",
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

