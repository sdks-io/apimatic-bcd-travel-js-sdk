
# Address 1

*This model accepts additional fields of type unknown.*

## Structure

`Address1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `city` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `region` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "Mahdentalstrasse 68.",
  "countryCode": "DE",
  "city": "Stuttgart",
  "postalCode": "71065",
  "region": "region8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

