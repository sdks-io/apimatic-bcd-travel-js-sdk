
# Leg 33

*This model accepts additional fields of type unknown.*

## Structure

`Leg33`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureAirportCode` | `string \| undefined` | Optional | - |
| `arrivalAirportCode` | `string \| undefined` | Optional | - |
| `flightNumber` | `string \| undefined` | Optional | - |
| `segmentNumber` | `number \| undefined` | Optional | - |
| `classOfServiceCode` | `string \| undefined` | Optional | - |
| `fareBasisCode` | `string \| undefined` | Optional | - |
| `departureDate` | `string \| undefined` | Optional | - |
| `arrivalDate` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "departureAirportCode": "SEA",
  "arrivalAirportCode": "DEN",
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

