
# Air 16

*This model accepts additional fields of type unknown.*

## Structure

`Air16`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `taxes` | [`Taxis1[]`](../../doc/models/taxis-1.md) | Required | - |
| `tickets` | [`Ticket32[]`](../../doc/models/ticket-32.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
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
          "arrivalAirportCode": "arrivalAirportCode6",
          "flightNumber": "flightNumber8",
          "segmentNumber": 94,
          "classOfServiceCode": "classOfServiceCode0",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        },
        {
          "departureAirportCode": "departureAirportCode2",
          "arrivalAirportCode": "arrivalAirportCode6",
          "flightNumber": "flightNumber8",
          "segmentNumber": 94,
          "classOfServiceCode": "classOfServiceCode0",
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

