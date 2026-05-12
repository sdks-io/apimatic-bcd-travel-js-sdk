
# Line Item

*This model accepts additional fields of type unknown.*

## Structure

`LineItem`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `sequenceNumber` | `number \| undefined` | Optional | - |
| `description` | `string \| undefined` | Optional | - |
| `total` | [`LineItemTotal \| undefined`](../../doc/models/containers/line-item-total.md) | Optional | This is a container for one-of cases. |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "sequenceNumber": 118,
  "description": "description6",
  "total": 230,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

