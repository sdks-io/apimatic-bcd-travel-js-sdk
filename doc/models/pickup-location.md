
# Pickup Location

*This model accepts additional fields of type unknown.*

## Structure

`PickupLocation`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `countryCode` | `string` | Required | - |
| `address2` | `string \| undefined` | Optional | - |
| `city` | `string \| undefined` | Optional | - |
| `region` | `string \| undefined` | Optional | - |
| `postalCode` | `string \| undefined` | Optional | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
  "countryCode": "DE",
  "address2": "address28",
  "city": "city4",
  "region": "region2",
  "postalCode": "postalCode2",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

