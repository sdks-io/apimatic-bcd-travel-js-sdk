
# Fare 5

*This model accepts additional fields of type unknown.*

## Structure

`Fare5`

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
  "amount": 802,
  "currencyCode": "USD",
  "description": "Estimated Total",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

