
# Line Item 1

*This model accepts additional fields of type unknown.*

## Structure

`LineItem1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `sequenceNumber` | `number` | Required | - |
| `description` | `string \| undefined` | Optional | - |
| `total` | [`LineItem1Total`](../../doc/models/containers/line-item-1-total.md) | Required | This is a container for one-of cases. |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "sequenceNumber": 222,
  "description": "description6",
  "total": 22,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

