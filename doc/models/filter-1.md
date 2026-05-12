
# Filter 1

*This model accepts additional fields of type unknown.*

## Structure

`Filter1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `recordLocator` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "recordLocator": [
    "EKDCAG"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

