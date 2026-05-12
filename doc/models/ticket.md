
# Ticket

*This model accepts additional fields of type unknown.*

## Structure

`Ticket`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `legs` | [`TicketLegs[]`](../../doc/models/containers/ticket-legs.md) | Required | This is Array of a container for one-of cases. |
| `invoiceNumber` | `string` | Required | - |
| `isConjunctive` | `boolean \| undefined` | Optional | - |
| `validatingCarrier` | `string` | Required | - |
| `ticketStatus` | `string` | Required | - |
| `calculatedTicketStatus` | `string` | Required | - |
| `taxes` | [`Taxis1[]`](../../doc/models/taxis-1.md) | Required | - |
| `ticketNumber` | `string` | Required | - |
| `recordLocator` | `string \| undefined` | Optional | - |
| `issueDateTime` | `string` | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `fare` | [`Fare`](../../doc/models/fare.md) | Required | - |
| `payments` | [`Payment1[]`](../../doc/models/payment-1.md) | Required | - |
| `lineItems` | `string[]` | Required | - |
| `bookingType` | `string` | Required | - |
| `passenger` | [`Passenger`](../../doc/models/passenger.md) | Required | - |
| `isInternational` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
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
    }
  ],
  "invoiceNumber": "invoiceNumber0",
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
    "lineItems8",
    "lineItems9"
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
  "isConjunctive": false,
  "recordLocator": "recordLocator4",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

