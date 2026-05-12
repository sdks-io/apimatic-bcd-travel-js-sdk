
# Drop Off Location 1

*This model accepts additional fields of type unknown.*

## Structure

`DropOffLocation1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `address2` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `city` | `string` | Required | - |
| `region` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "Hertz San Francisco International Airport",
  "address2": "780 McDonnell Road",
  "countryCode": "US",
  "city": "San Francisco",
  "region": "California",
  "postalCode": "94128",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

