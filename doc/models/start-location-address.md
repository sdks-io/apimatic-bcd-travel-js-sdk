
# Start Location Address

*This model accepts additional fields of type unknown.*

## Structure

`StartLocationAddress`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `address2` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `city` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "14 COPE CT HILLSBOROUGH",
  "address2": "27 NOPE ST WILLSBOROUGH",
  "countryCode": "CE",
  "city": "LHR",
  "postalCode": "555444",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

