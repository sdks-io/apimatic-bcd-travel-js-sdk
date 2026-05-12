
# Address 32

*This model accepts additional fields of type unknown.*

## Structure

`Address32`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `addressCountryCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "addressCountryCode": "US",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

