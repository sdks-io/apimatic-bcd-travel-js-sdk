
# Airretrieve Reservations List Request

## Structure

`AirretrieveReservationsListRequest`

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
| `currency` | `string` | Required | - |

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
  "traveler_email": "rkaydanowski+hcat@bcdtriptech.com",
  "limit": 10,
  "offset": 11,
  "currency": "UAH"
}
```

