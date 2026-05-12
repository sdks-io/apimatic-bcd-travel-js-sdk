
# End Location Address

*This model accepts additional fields of type unknown.*

## Structure

`EndLocationAddress`

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
  "address1": "EWR AIRPORT UA 2310",
  "address2": "EWR AIRPORT UA 2511",
  "countryCode": "AE",
  "city": "Dubai",
  "postalCode": "779944",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

