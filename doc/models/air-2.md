
# Air 2

*This model accepts additional fields of type unknown.*

## Structure

`Air2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `id` | `string` | Required | - |
| `taxes` | [`Taxis1[]`](../../doc/models/taxis-1.md) | Required | - |
| `tickets` | [`Ticket4[]`](../../doc/models/ticket-4.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "id": "id6",
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
          "departureAirportCode": "departureAirportCode2",
          "departureDateTime": "departureDateTime4",
          "arrivalAirportCode": "arrivalAirportCode6",
          "arrivalDateTime": "arrivalDateTime8",
          "flightNumber": "flightNumber8",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        {
          "departureAirportCode": "departureAirportCode2",
          "departureDateTime": "departureDateTime4",
          "arrivalAirportCode": "arrivalAirportCode6",
          "arrivalDateTime": "arrivalDateTime8",
          "flightNumber": "flightNumber8",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "invoiceNumber": "invoiceNumber0",
      "isConjunctive": false,
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
          "amount": 5176.57,
          "paymentType": "Credit Card",
          "currencyCode": "USD",
          "cardDetail": {
            "type": "VI",
            "number": "9484",
            "exampleAdditionalProperty": {
              "key1": "val1",
              "key2": "val2"
            }
          },
          "authorizationCode": "004511",
          "ticketNumber": "ticketNumber4",
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
      "recordLocator": "recordLocator4",
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

