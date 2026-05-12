
# Hotelsupdate Reservation Details Request 1

*This model accepts additional fields of type unknown.*

## Structure

`HotelsupdateReservationDetailsRequest1`

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
| `configurationId` | `number` | Required | - |
| `system` | `string` | Required | - |
| `bookingUid` | `string` | Required | - |
| `bookingData` | [`BookingData`](../../doc/models/booking-data.md) | Required | - |
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
  "configuration_id": 4,
  "system": "aft",
  "booking_uid": "dc2ee73lfjykj4zliaqlm5xix",
  "booking_data": {
    "is_ghost": false,
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

