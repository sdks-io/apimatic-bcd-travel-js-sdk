
# Filter 13

*This model accepts additional fields of type unknown.*

## Structure

`Filter13`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ticketStatus` | `string[]` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "ticketStatus": [
    "TICKETED"
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

