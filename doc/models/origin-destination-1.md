
# Origin Destination 1

*This model accepts additional fields of type unknown.*

## Structure

`OriginDestination1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureDate` | `string` | Required | - |
| `departureLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `arrivalLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `timeRestriction` | [`TimeRestriction \| undefined`](../../doc/models/time-restriction.md) | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "departure_date": "2023-09-11",
  "departure_location": {
    "location_code": "LIS",
    "location_type": "airport",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "arrival_location": {
    "location_code": "AMS",
    "location_type": "airport",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "time_restriction": {
    "time": "12:00",
    "time_type": "departure",
    "time_window": 12,
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

