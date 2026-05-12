
# Cruise Ferry

*This model accepts additional fields of type unknown.*

## Structure

`CruiseFerry`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `reservations` | [`Reservation2[]`](../../doc/models/reservation-2.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "bcd3cccf-cb0e-cdb6-fa43-3ff021802350",
  "reservations": [
    {
      "bookingDateTime": "2022-02-11T09:19:00Z",
      "cabin": "TURISTAFLEXIBLE",
      "confirmationNumber": "4561",
      "endDateTime": "2022-03-01T08:00:00Z",
      "fare": {
        "amount": 802,
        "currencyCode": "USD",
        "description": "Estimated Total",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "linkCode": "A",
      "segmentNumber": 10,
      "shipName": "Angelena",
      "startDateTime": "2022-02-15T09:45:00Z",
      "vendorChainCode": "repudiandae",
      "vendorChainName": "erat",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

