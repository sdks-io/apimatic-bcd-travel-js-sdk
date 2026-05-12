
# Ticket 2

*This model accepts additional fields of type unknown.*

## Structure

`Ticket2`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `legs` | [`Leg3[]`](../../doc/models/leg-3.md) | Required | - |
| `invoiceNumber` | `string \| undefined` | Optional | - |
| `validatingCarrier` | `string` | Required | - |
| `ticketStatus` | `string` | Required | - |
| `calculatedTicketStatus` | `string` | Required | - |
| `taxes` | [`Taxis4[]`](../../doc/models/taxis-4.md) | Required | - |
| `ticketNumber` | `string` | Required | - |
| `recordLocator` | `string` | Required | - |
| `issueDateTime` | `string` | Required | - |
| `bookingDateTime` | `string` | Required | - |
| `fare` | [`Fare`](../../doc/models/fare.md) | Required | - |
| `payments` | [`Payment3[]`](../../doc/models/payment-3.md) | Required | - |
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
  "validatingCarrier": "validatingCarrier8",
  "ticketStatus": "ticketStatus4",
  "calculatedTicketStatus": "calculatedTicketStatus2",
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
  "ticketNumber": "ticketNumber0",
  "recordLocator": "recordLocator2",
  "issueDateTime": "issueDateTime6",
  "bookingDateTime": "bookingDateTime0",
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
    "lineItems6",
    "lineItems7"
  ],
  "bookingType": "bookingType8",
  "passenger": {
    "firstName": "FIRSTNAME",
    "lastName": "NONAME",
    "exampleAdditionalProperty": {
      "key1": "val1",
      "key2": "val2"
    }
  },
  "isInternational": false,
  "invoiceNumber": "invoiceNumber8",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

