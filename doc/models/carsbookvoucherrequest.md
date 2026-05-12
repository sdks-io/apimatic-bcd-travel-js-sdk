
# Carsbookvoucherrequest

## Structure

`Carsbookvoucherrequest`

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
| `booktrackId` | `string` | Required | - |
| `rateKey` | `string` | Required | - |
| `bookerEmail` | `string` | Required | - |
| `bookerFirstName` | `string` | Required | - |
| `bookerLastName` | `string` | Required | - |
| `travelerEmail` | `string` | Required | - |
| `travelerFirstName` | `string` | Required | - |
| `travelerLastName` | `string` | Required | - |
| `pnrId` | `string` | Required | - |
| `paymentMethod` | `string` | Required | - |
| `billingNumber` | `string` | Required | - |
| `billingReference` | `string` | Required | - |

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
  "booktrack_id": "{{timestamp}}",
  "rate_key": "HXTA-wctTtPdSwR0YwTgxf-sQC0HtnMUY1LzJK9VGCdQejcoM_APOabKwHM6imiVD9poTZnXqc_fCWoi879kxynYmjEJ4Gmxy07E4lOfYJ5JJiunbu1l3SiNnbmADGS5WO4DhWZhMu6uIvkWf1zRsQ9twRN5z4_KrWKQJTCjMvQCNnY05OuSXKEldTrJSW-Ge2cqDE8DRAf-f3keu9jxwLy8KGihqmY1_zTAaaPHyOqRQnA88a2laCR8k7SmcMdzMdzB_h7OJqsF0opsrM3x_g6oN54-s9DJXLe0ohbrdNsgscJd0s2EzurxHNFgh2M8taFPJE4WEjBBK0qJqVXovnVCE0UXYJDdKXUYmnBmm2o9t_MMtNkfYPrWZF2vJQC-NNiWqqDa9kKm9jTeQxbnQH0qOaAkDlASm08aFsa_Bq-NZTLcKKUtxENAXSe1pP2p2OK3vwmN0jgLnIocWHXHQMT1Tov7X0dhv1Qd-yK5d__gi6v6tcv2pREKYg_RABmzsvEc7Qk6e-HDm-A-Vs5xZaLuD2O49_4kaE7t2UbiXezGw8h8g4Wg0GL3kpPFTrbNBwqBh_mCUCoGk-dRDs3XSiVtLv9GhkvF8C7MLL0nvKOORdi8hCyabkda79vj0wPUJnzMI7jebOR7p2TKRRnaKYC4bS8PCOusNEGxw276XUne0mkapAe3ziw=",
  "booker_email": "booker@bcdtriptech.com",
  "booker_first_name": "BookerFirst",
  "booker_last_name": "BookerLast",
  "traveler_email": "traveler@bcdtriptech.com",
  "traveler_first_name": "TravelerFirst",
  "traveler_last_name": "TravelerLast",
  "pnr_id": "NQ86M3",
  "payment_method": "voucher",
  "billing_number": "A123456",
  "billing_reference": "qwerty"
}
```

