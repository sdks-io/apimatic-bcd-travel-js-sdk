
# Search Expensesbyrecord Locator Request

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyrecordLocatorRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filter` | [`Filter1`](../../doc/models/filter-1.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "limit": 10,
  "offset": 0,
  "filter": {
    "recordLocator": [
      "EKDCAG"
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

