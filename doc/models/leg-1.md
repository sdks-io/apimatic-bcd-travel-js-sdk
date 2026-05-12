
# Leg 1

*This model accepts additional fields of type unknown.*

## Structure

`Leg1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureAirportCode` | `string \| undefined` | Optional | - |
| `departureDateTime` | `string \| undefined` | Optional | - |
| `arrivalAirportCode` | `string \| undefined` | Optional | - |
| `arrivalDateTime` | `string \| undefined` | Optional | - |
| `flightNumber` | `string \| undefined` | Optional | - |
| `segmentNumber` | `number \| undefined` | Optional | - |
| `classOfServiceCode` | `string \| undefined` | Optional | - |
| `fareBasisCode` | `string \| undefined` | Optional | - |
| `marketingAirlineCode` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "departureAirportCode": "SEA",
  "departureDateTime": "2022-02-27T11:00:00Z",
  "arrivalAirportCode": "DEN",
  "arrivalDateTime": "2022-02-27T14:46:00Z",
  "flightNumber": "1630",
  "segmentNumber": 1,
  "classOfServiceCode": "Z",
  "fareBasisCode": "JAR1",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

