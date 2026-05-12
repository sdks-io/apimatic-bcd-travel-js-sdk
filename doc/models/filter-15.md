
# Filter 15

*This model accepts additional fields of type unknown.*

## Structure

`Filter15`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `hasTransaction` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "hasTransaction": true,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

