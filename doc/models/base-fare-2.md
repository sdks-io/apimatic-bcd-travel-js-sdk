
# Base Fare 2

*This model accepts additional fields of type unknown.*

## Structure

`BaseFare2`

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
  "amount": 10.77,
  "currencyCode": "USD",
  "description": "Base Fare",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

