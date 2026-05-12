
# Air 1

*This model accepts additional fields of type unknown.*

## Structure

`Air1`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `taxes` | [`Taxis4[]`](../../doc/models/taxis-4.md) | Required | - |
| `tickets` | [`Ticket2[]`](../../doc/models/ticket-2.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "id4",
  "taxes": [
    {
      "name": "name0",
      "code": "code8",
      "amount": 50,
      "currencyCode": "currencyCode0",
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "tickets": [
    {
      "legs": [
        {
          "departureAirportCode": "BER",
          "departureDateTime": "2022-02-15T09:45:00Z",
          "arrivalAirportCode": "FRA",
          "arrivalDateTime": "2022-02-15T10:55:00Z",
          "flightNumber": "179",
          "segmentNumber": 1,
          "marketingAirlineCode": "LH",
          "classOfServiceCode": "S",
          "fareBasisCode": "SLNCD8",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "validatingCarrier": "validatingCarrier0",
      "ticketStatus": "ticketStatus6",
      "calculatedTicketStatus": "calculatedTicketStatus4",
      "taxes": [
        {
          "name": "name0",
          "code": "code8",
          "amount": 50,
          "currencyCode": "currencyCode0",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "ticketNumber": "ticketNumber2",
      "recordLocator": "recordLocator4",
      "issueDateTime": "issueDateTime8",
      "bookingDateTime": "bookingDateTime8",
      "fare": {
        "amount": 5176.57,
        "currencyCode": "USD",
        "description": "Total Fare",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "payments": [
        {
          "amount": 942.07,
          "paymentType": "Credit Card",
          "currencyCode": "EUR",
          "cardDetail": {
            "type": "CA",
            "number": "1234",
            "exampleAdditionalProperty": {
              "key1": "val1",
              "key2": "val2"
            }
          },
          "authorizationCode": "01010 C",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "lineItems": [
        "lineItems8"
      ],
      "bookingType": "bookingType6",
      "passenger": {
        "firstName": "FIRSTNAME",
        "lastName": "NONAME",
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
      "isInternational": false,
      "invoiceNumber": "invoiceNumber0",
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

