
# Search Expensesbycalculated Ticket Status Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbycalculatedTicketStatusRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter14`](../../doc/models/filter-14.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 2,
  "offset": 0,
  "filter": {
    "calculatedTicketStatus": [
      "USED/FLOWN",
      "EXPIRED"
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

