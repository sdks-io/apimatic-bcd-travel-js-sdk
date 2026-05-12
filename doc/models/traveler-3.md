
# Traveler 3

## Structure

`Traveler3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ffNumbers` | [`FfNumber[]`](../../doc/models/ff-number.md) | Required | - |
| `travelerName` | [`TravelerName`](../../doc/models/traveler-name.md) | Required | - |

## Example (as JSON)

```json
{
  "ff_numbers": [
    {
      "airline_code": "DI",
      "ff_number": "222222"
    },
    {
      "airline_code": "KL",
      "ff_number": "333333"
    }
  ],
  "traveler_name": {
    "first_name": "Darth",
    "last_name": "Vader"
  }
}
```

