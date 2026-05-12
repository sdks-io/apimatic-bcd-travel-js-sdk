
# Taxis 1

*This model accepts additional fields of type unknown.*

## Structure

`Taxis1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string` | Required | - |
| `code` | `string` | Required | - |
| `amount` | [`Taxis1Amount`](../../doc/models/containers/taxis-1-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name6",
  "code": "code4",
  "amount": 222,
  "currencyCode": "currencyCode6",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

