
# Traveler

## Structure

`Traveler`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `travelerType` | `string` | Required | - |
| `ffNumbers` | [`FfNumber[]`](../../doc/models/ff-number.md) | Required | - |

## Example (as JSON)

```json
{
  "traveler_type": "adult",
  "ff_numbers": [
    {
      "airline_code": "KL",
      "ff_number": "1234321"
    }
  ]
}
```

