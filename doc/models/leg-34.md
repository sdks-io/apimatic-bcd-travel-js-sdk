
# Leg 34

*This model accepts additional fields of type unknown.*

## Structure

`Leg34`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `arrivalDateTime` | `string` | Required | - |
| `arrivalStationCode` | `string` | Required | - |
| `carrierCode` | `string` | Required | - |
| `carrierName` | `string` | Required | - |
| `departureDateTime` | `string` | Required | - |
| `departureStationCode` | `string` | Required | - |
| `segmentNumber` | `string` | Required | - |
| `trainNumber` | `string` | Required | - |
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
  "segmentNumber": "3",
  "trainNumber": "3410",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

