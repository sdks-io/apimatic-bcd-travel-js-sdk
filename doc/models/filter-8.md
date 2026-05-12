
# Filter 8

*This model accepts additional fields of type unknown.*

## Structure

`Filter8`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lastModifiedDateTime` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lastModifiedDateTime": "2022-02-01T21:12 TO 2022-02-17T10:40",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

