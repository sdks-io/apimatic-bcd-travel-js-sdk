
# Search Expensesbyglobal Customer Number Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyglobalCustomerNumberRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter11`](../../doc/models/filter-11.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 2,
  "offset": 0,
  "filter": {
    "globalCustomerNumber": [
      "9999",
      "20109999"
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

