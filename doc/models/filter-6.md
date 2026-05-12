
# Filter 6

*This model accepts additional fields of type unknown.*

## Structure

`Filter6`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `invoiceDateTime` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "invoiceDateTime": "2022-01-01T00:01 TO 2022-02-17T00:01",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

