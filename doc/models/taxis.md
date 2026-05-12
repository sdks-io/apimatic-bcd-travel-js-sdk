
# Taxis

*This model accepts additional fields of type unknown.*

## Structure

`Taxis`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `productId` | `string` | Required | - |
| `name` | `string` | Required | - |
| `code` | `string` | Required | - |
| `amount` | [`TaxisAmount`](../../doc/models/containers/taxis-amount.md) | Required | This is a container for one-of cases. |
| `currencyCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "productId": "productId2",
  "name": "name8",
  "code": "code6",
  "amount": 130,
  "currencyCode": "currencyCode8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

