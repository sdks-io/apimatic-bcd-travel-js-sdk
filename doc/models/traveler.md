
# Traveler

*This model accepts additional fields of type unknown.*

## Structure

`Traveler`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `travelerType` | `string` | Required | - |
| `ffNumbers` | [`FfNumber[]`](../../doc/models/ff-number.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "traveler_type": "adult",
  "ff_numbers": [
    {
      "airline_code": "KL",
      "ff_number": "1234321",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

