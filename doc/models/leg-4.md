
# Leg 4

*This model accepts additional fields of type unknown.*

## Structure

`Leg4`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `arrivalDateTime` | `string` | Required | - |
| `arrivalStationCode` | `string` | Required | - |
| `carrierCode` | `string` | Required | - |
| `carrierName` | `string` | Required | - |
| `classOfServiceCode` | `string` | Required | - |
| `departureDateTime` | `string` | Required | - |
| `departureStationCode` | `string` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `trainNumber` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "arrivalDateTime": "2022-03-09T10:06:00Z",
  "arrivalStationCode": "QDU",
  "carrierCode": "LH",
  "carrierName": "Lufthansa",
  "classOfServiceCode": "S",
  "departureDateTime": "2022-03-09T08:42:00Z",
  "departureStationCode": "FRA",
  "segmentNumber": 13,
  "trainNumber": "3502",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

