
# Drop Off Location 16

*This model accepts additional fields of type unknown.*

## Structure

`DropOffLocation16`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `address1` | `string` | Required | - |
| `addressCountryCode` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
  "addressCountryCode": "DE",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

