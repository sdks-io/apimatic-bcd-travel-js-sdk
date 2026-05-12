
# Traveler 3

*This model accepts additional fields of type unknown.*

## Structure

`Traveler3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ffNumbers` | [`FfNumber[]`](../../doc/models/ff-number.md) | Required | - |
| `travelerName` | [`TravelerName`](../../doc/models/traveler-name.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "ff_numbers": [
    {
      "airline_code": "DI",
      "ff_number": "222222",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    },
    {
      "airline_code": "KL",
      "ff_number": "333333",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "traveler_name": {
    "first_name": "Darth",
    "last_name": "Vader",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

