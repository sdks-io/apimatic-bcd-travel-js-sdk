
# Address 33

*This model accepts additional fields of type unknown.*

## Structure

`Address33`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `addressCountryCode` | `string` | Required | - |
| `addressLocality` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "Mahdentalstrasse 68.",
  "addressCountryCode": "DE",
  "addressLocality": "Stuttgart",
  "postalCode": "71065",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

