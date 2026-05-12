
# Specific Flight

*This model accepts additional fields of type unknown.*

## Structure

`SpecificFlight`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `airlineCode` | `string` | Required | - |
| `flightNumber` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "airline_code": "BA",
  "flight_number": "950",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

