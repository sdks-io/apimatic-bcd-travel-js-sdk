
# Traveler 1

*This model accepts additional fields of type unknown.*

## Structure

`Traveler1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `firstName` | `string` | Required | - |
| `lastName` | `string` | Required | - |
| `emailAddress` | `string` | Required | - |
| `identifiers` | `string[]` | Required | - |
| `profileStatus` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "firstName": "FIRSTNAME",
  "lastName": "NONAME",
  "emailAddress": "FIRSTNAME.NONAME@COMPANY.COM",
  "identifiers": [],
  "profileStatus": "Active",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

