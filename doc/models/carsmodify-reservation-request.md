
# Carsmodify Reservation Request

*This model accepts additional fields of type unknown.*

## Structure

`CarsmodifyReservationRequest`

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
| `flightNumber` | `string` | Required | - |
| `specialEquipment` | `string[]` | Required | - |
| `specialInformation` | `string` | Required | - |
| `pickupDatetime` | `string` | Required | - |
| `dropoffDatetime` | `string` | Required | - |
| `carType` | `string` | Required | - |
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
  "booking_uid": "{{booking_uid}}",
  "flight_number": "AA1234",
  "special_equipment": [
    "CSI"
  ],
  "special_information": "I want a blue car",
  "pickup_datetime": "2019-02-25T11:15",
  "dropoff_datetime": "2019-02-27T10:30",
  "car_type": "ECAR",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

