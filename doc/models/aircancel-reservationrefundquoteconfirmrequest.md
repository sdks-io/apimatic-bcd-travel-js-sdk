
# Aircancel Reservationrefundquoteconfirmrequest

*This model accepts additional fields of type unknown.*

## Structure

`AircancelReservationrefundquoteconfirmrequest`

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
| `email` | `string` | Required | - |
| `refundQuoteId` | `string` | Required | - |
| `bookingUid` | `string` | Required | - |
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
  "email": "booker@bcdtriptech.com",
  "refund_quote_id": "insert_quote_id_here",
  "booking_uid": "63a36d2c2d4d55f488e097c2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

