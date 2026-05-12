
# Search Expensesbyaccount Id Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyaccountIdRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter10`](../../doc/models/filter-10.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 2,
  "offset": 0,
  "filter": {
    "accountId": [
      "999999901",
      "999999902"
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

