
# Address 3

*This model accepts additional fields of type unknown.*

## Structure

`Address3`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `city` | `string` | Required | - |
| `region` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "47000 Lakeview Blvd",
  "countryCode": "US",
  "city": "Fremont",
  "region": "California",
  "postalCode": "94538",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

