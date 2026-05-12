
# Time Restriction

*This model accepts additional fields of type unknown.*

## Structure

`TimeRestriction`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `time` | `string` | Required | - |
| `timeType` | `string` | Required | - |
| `timeWindow` | `number` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "time": "12:00",
  "time_type": "departure",
  "time_window": 12,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

