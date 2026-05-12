
# Airavailabilityrequest

*This model accepts additional fields of type unknown.*

## Structure

`Airavailabilityrequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `apiKey` | `string` | Required | - |
| `timestamp` | `string` | Required | - |
| `nonce` | `string` | Required | - |
| `locale` | `string` | Required | - |
| `customerIp` | `string` | Required | - |
| `sessionId` | `string` | Required | - |
| `userAgent` | `string` | Required | - |
| `system` | `string` | Required | - |
| `configurationId` | `number` | Required | - |
| `originDestinations` | [`OriginDestination[]`](../../doc/models/origin-destination.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "api_key": "{{ASB_API_KEY}}",
  "timestamp": "{{timestamp}}",
  "nonce": "{{nonce}}",
  "locale": "en_US",
  "customer_ip": "127.0.0.1",
  "session_id": "{{session_id}}",
  "user_agent": "curl/7.64.0",
  "system": "aft",
  "configuration_id": 4,
  "origin_destinations": [
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
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

