
# Ff Number

*This model accepts additional fields of type unknown.*

## Structure

`FfNumber`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `airlineCode` | `string` | Required | - |
| `ffNumber` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "airline_code": "KL",
  "ff_number": "1234321",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

