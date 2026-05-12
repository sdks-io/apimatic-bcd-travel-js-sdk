
# Carsretrieve Reservations List Request

*This model accepts additional fields of type unknown.*

## Structure

`CarsretrieveReservationsListRequest`

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
| `travelerEmail` | `string` | Required | - |
| `limit` | `number` | Required | - |
| `offset` | `number` | Required | - |
| `filters` | `unknown` | Required | - |
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
  "traveler_email": "traveler@bcdtriptech.com",
  "limit": 20,
  "offset": 0,
  "filters": {},
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

