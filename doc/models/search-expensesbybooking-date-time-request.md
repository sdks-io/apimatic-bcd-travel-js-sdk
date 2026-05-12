
# Search Expensesbybooking Date Time Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbybookingDateTimeRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter4`](../../doc/models/filter-4.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 1,
  "offset": 0,
  "filter": {
    "bookingDateTime": "2022-02-11",
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

