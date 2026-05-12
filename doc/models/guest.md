
# Guest

*This model accepts additional fields of type unknown.*

## Structure

`Guest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `lastName` | `string` | Required | - |
| `identifiers` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "lastName": "NONAME FIRSTNAME",
  "identifiers": [],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

