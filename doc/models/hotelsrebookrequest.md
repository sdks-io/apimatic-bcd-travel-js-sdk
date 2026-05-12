
# Hotelsrebookrequest

*This model accepts additional fields of type unknown.*

## Structure

`Hotelsrebookrequest`

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
| `bookingUid` | `string` | Required | - |
| `booktrackId` | `string` | Required | - |
| `hotelId` | `number` | Required | - |
| `originalCurrency` | `string` | Required | - |
| `originalTotal` | `number` | Required | - |
| `rateKey` | `string` | Required | - |
| `bookerEmail` | `string` | Required | - |
| `bookerFirstName` | `string` | Required | - |
| `bookerLastName` | `string` | Required | - |
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
  "booking_uid": "dc2ee73lfjykj4zliaqlm5xix",
  "booktrack_id": "{{timestamp}}",
  "hotel_id": 574889,
  "original_currency": "USD",
  "original_total": 229.15,
  "rate_key": "eJxNjMtOwzAURPf9ivsBTWubvDq768SKrSaxFTtFsKtEFyBYQf8fp2yY1TyORgmlCtEWTzIJCVWhqg+lapVsgRKomrJtT4C1eGgArl/Xt9v9e+uCHWtZAWHxAIuSRQ6DPANKKFmIppDyn1eAtv0+0/vX+nFo1gVYYw/IU3PYgD993D/fbz/5k5li4hfiuafIF7OTdHbzQJPXbnQpD11nYnR6NPR8JM3JplXvOj8Fso5iMKYnNyezzCbRkTiETLrAW0uL99MvQXY/vQ==",
  "booker_email": "booker@bcdtriptech.com",
  "booker_first_name": "BookerFirst",
  "booker_last_name": "BookerLast",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

