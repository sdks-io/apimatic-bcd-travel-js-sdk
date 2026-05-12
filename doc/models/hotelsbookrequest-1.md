
# Hotelsbookrequest 1

*This model accepts additional fields of type unknown.*

## Structure

`Hotelsbookrequest1`

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
| `checkin` | `string` | Required | - |
| `checkout` | `string` | Required | - |
| `currency` | `string` | Required | - |
| `booktrackId` | `string` | Required | - |
| `guestCount` | `number` | Required | - |
| `hotelId` | `number` | Required | - |
| `originalCurrency` | `string` | Required | - |
| `originalTotal` | `number` | Required | - |
| `rateKey` | `string` | Required | - |
| `bookerEmail` | `string` | Required | - |
| `bookerFirstName` | `string` | Required | - |
| `bookerLastName` | `string` | Required | - |
| `travelerEmail` | `string` | Required | - |
| `travelerFirstName` | `string` | Required | - |
| `travelerLastName` | `string` | Required | - |
| `paymentMethod` | `string` | Required | - |
| `loyaltyCardChainCode` | `string` | Required | - |
| `loyaltyCardNumber` | `string` | Required | - |
| `creditCardNumber` | `string` | Required | - |
| `creditCardExpirationYear` | `string` | Required | - |
| `creditCardExpirationMonth` | `string` | Required | - |
| `creditCardFirstName` | `string` | Required | - |
| `creditCardLastName` | `string` | Required | - |
| `creditCardAddress` | `string` | Required | - |
| `creditCardCountryCode` | `string` | Required | - |
| `creditCardCity` | `string` | Required | - |
| `creditCardStateProvinceCode` | `string` | Required | - |
| `creditCardPostalCode` | `string` | Required | - |
| `creditCardPhone` | `string` | Required | - |
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
  "checkin": "2021-07-11",
  "checkout": "2021-07-12",
  "currency": "USD",
  "booktrack_id": "{{timestamp}}",
  "guest_count": 1,
  "hotel_id": 574889,
  "original_currency": "USD",
  "original_total": 229.15,
  "rate_key": "eJxNjM0SwUAQhO+eYh5A2Bn5WX0bdsumkGwloYqbKg4UJ7y/hIs+dX/d1WJEEmOTGXeGIRmyfJKKFbZACmRFau0cCAFfrYDT43S+vJ8Di2GTcwbEpgbUiJo+LHgNiBFOTJEw/3npy+DG/Xp8zL+HftcAu9YBPC8mw+Cn2/t+vbz6T1VqOz2QVo5a3fsR07qsVrTwbrSst5FCSW303lFZdb6pfEdT0hg3nsqoA6WmrrcfzNk4Wg==",
  "booker_email": "booker@bcdtriptech.com",
  "booker_first_name": "BookerFirst",
  "booker_last_name": "BookerLast",
  "traveler_email": "traveler@bcdtriptech.com",
  "traveler_first_name": "TravelerFirst",
  "traveler_last_name": "TravelerLast",
  "payment_method": "card",
  "loyalty_card_chain_code": "RT",
  "loyalty_card_number": "1001709",
  "credit_card_number": "5555555555554444",
  "credit_card_expiration_year": "2030",
  "credit_card_expiration_month": "01",
  "credit_card_first_name": "GHOST",
  "credit_card_last_name": "CARD",
  "credit_card_address": "addr1",
  "credit_card_country_code": "US",
  "credit_card_city": "Atlanta",
  "credit_card_state_province_code": "GA",
  "credit_card_postal_code": "12345",
  "credit_card_phone": "1234567890",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

