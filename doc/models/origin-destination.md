
# Origin Destination

*This model accepts additional fields of type unknown.*

## Structure

`OriginDestination`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureDate` | `string` | Required | - |
| `departureLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `arrivalLocation` | [`DepartureLocation`](../../doc/models/departure-location.md) | Required | - |
| `specificFlights` | [`SpecificFlight[]`](../../doc/models/specific-flight.md) | Required | - |
| `airlineCodes` | `string[]` | Required | - |
| `timeRestriction` | [`TimeRestriction`](../../doc/models/time-restriction.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "departure_date": "2023-09-16",
  "departure_location": {
    "location_code": "LON",
    "location_type": "city",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "arrival_location": {
    "location_code": "MUC",
    "location_type": "city",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "specific_flights": [
    {
      "airline_code": "BA",
      "flight_number": "950",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "airline_codes": [
    "CJ",
    "BA"
  ],
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

