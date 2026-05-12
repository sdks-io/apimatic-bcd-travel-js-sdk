
# Fare 3

*This model accepts additional fields of type unknown.*

## Structure

`Fare3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | [`Fare3Amount`](../../doc/models/containers/fare-3-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `description` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 4574.77,
  "currencyCode": "USD",
  "description": "Total Fare",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

