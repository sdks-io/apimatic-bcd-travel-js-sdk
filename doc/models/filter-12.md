
# Filter 12

*This model accepts additional fields of type unknown.*

## Structure

`Filter12`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `customerNumber` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "customerNumber": [
    "9999999999"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

