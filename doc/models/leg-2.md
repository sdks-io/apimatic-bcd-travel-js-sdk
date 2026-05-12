
# Leg 2

*This model accepts additional fields of type unknown.*

## Structure

`Leg2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `arrivalDateTime` | `string` | Required | - |
| `arrivalStationCode` | `string` | Required | - |
| `carrierCode` | `string` | Required | - |
| `carrierName` | `string` | Required | - |
| `departureDateTime` | `string` | Required | - |
| `departureStationCode` | `string` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `trainNumber` | `string` | Required | - |
| `classOfServiceCode` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "arrivalDateTime": "2022-02-28T12:08:00Z",
  "arrivalStationCode": "ZWS",
  "carrierCode": "LH",
  "carrierName": "Lufthansa",
  "departureDateTime": "2022-02-28T10:52:00Z",
  "departureStationCode": "FRA",
  "segmentNumber": 3,
  "trainNumber": "3410",
  "classOfServiceCode": "classOfServiceCode0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

