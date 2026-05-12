
# Traveler 4

*This model accepts additional fields of type unknown.*

## Structure

`Traveler4`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `dateOfBirth` | `string` | Required | - |
| `gender` | `string` | Required | - |
| `travelerEmail` | `string` | Required | - |
| `travelerName` | [`TravelerName`](../../doc/models/traveler-name.md) | Required | - |
| `passport` | [`Passport`](../../doc/models/passport.md) | Required | - |
| `tspmTravelerId` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "date_of_birth": "2000-11-20",
  "gender": "M",
  "traveler_email": "traveler@bcdtriptech.com",
  "traveler_name": {
    "first_name": "TravelerFirst",
    "last_name": "TravelerLast",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "passport": {
    "country_of_issue": "UA",
    "expiry_date": "2029-09-12",
    "nationality": "UA",
    "number": "ZY123321",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "tspm_traveler_id": "24.9999999999995",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

