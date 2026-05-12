
# Leg 3

*This model accepts additional fields of type unknown.*

## Structure

`Leg3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `departureAirportCode` | `string` | Required | - |
| `departureDateTime` | `string \| undefined` | Optional | - |
| `arrivalAirportCode` | `string` | Required | - |
| `arrivalDateTime` | `string \| undefined` | Optional | - |
| `flightNumber` | `string` | Required | - |
| `segmentNumber` | `number` | Required | - |
| `marketingAirlineCode` | `string` | Required | - |
| `classOfServiceCode` | `string` | Required | - |
| `fareBasisCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "departureAirportCode": "BER",
  "departureDateTime": "2022-02-15T09:45:00Z",
  "arrivalAirportCode": "FRA",
  "arrivalDateTime": "2022-02-15T10:55:00Z",
  "flightNumber": "179",
  "segmentNumber": 1,
  "marketingAirlineCode": "LH",
  "classOfServiceCode": "S",
  "fareBasisCode": "SLNCD8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

