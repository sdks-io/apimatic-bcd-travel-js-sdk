
# Sort

*This model accepts additional fields of type unknown.*

## Structure

`Sort`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lastModifiedDateTime` | `string` | Required | - |
| `invoiceDateTime` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lastModifiedDateTime": "asc",
  "invoiceDateTime": "desc",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

