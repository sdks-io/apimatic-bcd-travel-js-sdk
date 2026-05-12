
# Search Expensesbytraveler Email Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbytravelerEmailRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter3`](../../doc/models/filter-3.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 10,
  "offset": 0,
  "filter": {
    "travelerEmail": [
      "JDOE@SOMEWHERE.COM"
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

