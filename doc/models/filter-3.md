
# Filter 3

*This model accepts additional fields of type unknown.*

## Structure

`Filter3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `travelerEmail` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "travelerEmail": [
    "JDOE@SOMEWHERE.COM"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

