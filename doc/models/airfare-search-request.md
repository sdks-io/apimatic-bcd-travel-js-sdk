
# Airfare Search Request

## Structure

`AirfareSearchRequest`

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
| `currency` | `string` | Required | - |
| `airlineCodes` | `string[]` | Required | - |
| `travelers` | [`Traveler[]`](../../doc/models/traveler.md) | Required | - |
| `originDestinations` | [`OriginDestination1[]`](../../doc/models/origin-destination-1.md) | Required | - |
| `includedBaggage` | `boolean` | Required | - |
| `changeableOnly` | `boolean` | Required | - |
| `refundableOnly` | `boolean` | Required | - |
| `excludePenalties` | `boolean` | Required | - |

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
  "currency": "EUR",
  "airline_codes": [
    "KL"
  ],
  "travelers": [
    {
      "traveler_type": "adult",
      "ff_numbers": [
        {
          "airline_code": "KL",
          "ff_number": "1234321"
        }
      ]
    }
  ],
  "origin_destinations": [
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
    },
    {
      "departure_date": "2023-09-12",
      "departure_location": {
        "location_code": "AMS",
        "location_type": "airport"
      },
      "arrival_location": {
        "location_code": "LIS",
        "location_type": "airport"
      },
      "time_restriction": {
        "time": "time2",
        "time_type": "time_type8",
        "time_window": 226
      }
    }
  ],
  "included_baggage": true,
  "changeable_only": false,
  "refundable_only": true,
  "exclude_penalties": true
}
```

