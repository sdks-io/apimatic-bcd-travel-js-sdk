
# Filter 11

*This model accepts additional fields of type unknown.*

## Structure

`Filter11`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `globalCustomerNumber` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "globalCustomerNumber": [
    "9999",
    "20109999"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

