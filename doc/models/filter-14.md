
# Filter 14

*This model accepts additional fields of type unknown.*

## Structure

`Filter14`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `calculatedTicketStatus` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "calculatedTicketStatus": [
    "USED/FLOWN",
    "EXPIRED"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

