
# Taxis 3

*This model accepts additional fields of type unknown.*

## Structure

`Taxis3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productId` | `string` | Required | - |
| `name` | `string \| undefined` | Optional | - |
| `code` | `string` | Required | - |
| `amount` | [`Taxis3Amount`](../../doc/models/containers/taxis-3-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "productId": "productId6",
  "name": "name2",
  "code": "code0",
  "amount": 8,
  "currencyCode": "currencyCode2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

