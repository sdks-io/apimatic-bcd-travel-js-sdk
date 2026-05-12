
# Base Fare

*This model accepts additional fields of type unknown.*

## Structure

`BaseFare`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | `number` | Required | - |
| `currencyCode` | `string` | Required | - |
| `description` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 100,
  "currencyCode": "EUR",
  "description": "Daily",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

