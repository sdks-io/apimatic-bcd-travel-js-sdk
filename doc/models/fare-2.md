
# Fare 2

*This model accepts additional fields of type unknown.*

## Structure

`Fare2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | [`Fare2Amount`](../../doc/models/containers/fare-2-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `description` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 158,
  "currencyCode": "currencyCode4",
  "description": "description6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

