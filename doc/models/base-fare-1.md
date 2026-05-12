
# Base Fare 1

*This model accepts additional fields of type unknown.*

## Structure

`BaseFare1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `amount` | [`BaseFare1Amount`](../../doc/models/containers/base-fare-1-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `description` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "amount": 142.3,
  "currencyCode": "EUR",
  "description": "Weekly",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

