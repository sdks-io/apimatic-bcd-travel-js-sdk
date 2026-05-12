
# Booking Data

*This model accepts additional fields of type unknown.*

## Structure

`BookingData`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `isGhost` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "is_ghost": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

