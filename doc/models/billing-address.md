
# Billing Address

*This model accepts additional fields of type unknown.*

## Structure

`BillingAddress`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `city` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `postalCode` | `string` | Required | - |
| `stateCode` | `string` | Required | - |
| `streetAddress1` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "city": "Atlanta",
  "country_code": "US",
  "postal_code": "30328",
  "state_code": "GA",
  "street_address1": "6 Concourse Pkwy Suite 2400",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

