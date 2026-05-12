
# Passport

*This model accepts additional fields of type unknown.*

## Structure

`Passport`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `countryOfIssue` | `string` | Required | - |
| `expiryDate` | `string` | Required | - |
| `nationality` | `string` | Required | - |
| `number` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "country_of_issue": "UA",
  "expiry_date": "2029-09-12",
  "nationality": "UA",
  "number": "ZY123321",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

