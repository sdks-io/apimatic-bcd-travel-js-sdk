
# Origin Destination 1

## Structure

`OriginDestination1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureDate` | `string` | Required | - |
| `departureLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `arrivalLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `timeRestriction` | [`TimeRestriction \| undefined`](../../doc/models/time-restriction.md) | Optional | - |

## Example (as JSON)

```json
{
  "departure_date": "2023-09-11",
  "departure_location": {
    "location_code": "LIS",
    "location_type": "airport"
  },
  "arrival_location": {
    "location_code": "AMS",
    "location_type": "airport"
  },
  "time_restriction": {
    "time": "12:00",
    "time_type": "departure",
    "time_window": 12
  }
}
```

