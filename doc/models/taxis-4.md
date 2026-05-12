
# Taxis 4

*This model accepts additional fields of type unknown.*

## Structure

`Taxis4`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `name` | `string \| undefined` | Optional | - |
| `code` | `string` | Required | - |
| `amount` | [`Taxis4Amount`](../../doc/models/containers/taxis-4-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "name": "name4",
  "code": "code2",
  "amount": 154,
  "currencyCode": "currencyCode4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

