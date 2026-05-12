
# Search Expensesbyticket Status Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyticketStatusRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter13`](../../doc/models/filter-13.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 2,
  "offset": 0,
  "filter": {
    "ticketStatus": [
      "TICKETED"
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

