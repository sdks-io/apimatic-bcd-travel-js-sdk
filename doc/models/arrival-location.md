
# Arrival Location

*This model accepts additional fields of type unknown.*

## Structure

`ArrivalLocation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `locationCode` | `string` | Required | - |
| `locationType` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "location_code": "MUC",
  "location_type": "city",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

