
# Search Expensesbycustomer Number

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbycustomerNumber`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `number` | Required | - |
| `status` | `string` | Required | - |
| `remainingRecords` | `number` | Required | - |
| `result` | [`Result2[]`](../../doc/models/result-2.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "code": 214,
  "status": "status6",
  "remainingRecords": 156,
  "result": [
    {
      "id": "id6",
      "total": 62.86,
      "taxesTotal": 68.62,
      "subtotal": 179.4,
      "currencyCode": "currencyCode6",
      "customerName": "customerName6",
      "globalCustomerNumber": "globalCustomerNumber4",
      "accountId": "accountId6",
      "customerNumber": "customerNumber8",
      "isInternational": false,
      "recordLocator": "recordLocator0",
      "lastModifiedDateTime": "lastModifiedDateTime0",
      "version": 236,
      "approvals": [
        "approvals3",
        "approvals4"
      ],
      "travelers": [
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
      ],
      "brokers": [
        {
          "name": "BCD Travel",
          "location": {
            "address": {
              "countryCode": "US",
              "exampleAdditionalProperty": {
                "key1": "val1",
                "key2": "val2"
              }
            },
            "exampleAdditionalProperty": {
              "key1": "val1",
              "key2": "val2"
            }
          },
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "sellers": [
        {
          "name": "Lufthansa",
          "validatingCarrier": "LH",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "payments": [
        {
          "productId": "5b25731f-b4b9-d5e3-e076-381257310431",
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
      "taxes": [
        {
          "productId": "productId4",
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
      "products": {
        "air": {
          "id": "id8",
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
        },
        "car": {
          "id": "bdfabb0e-2968-893e-7da1-97f18780193b",
          "reservations": [
            {
              "bookingDateTime": "2022-01-06T17:03:00Z",
              "carType": "Compact 4DR Car Manual AC",
              "confirmationNumber": "9917132564",
              "dropOffLocation": {
                "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
                "countryCode": "DE",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "endDateTime": "2022-03-03T17:00:00Z",
              "fare": {
                "amount": 400.95,
                "currencyCode": "EUR",
                "description": "Estimated Total",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "baseFare": {
                "amount": 100,
                "currencyCode": "EUR",
                "description": "Daily",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "isInternational": false,
              "lineItems": [],
              "numberOfCars": 1,
              "pickupLocation": {
                "address1": "Sixt Stuttgart Central Train Station\nArnulf-Klett-Platz 2\nStuttgart\n70173",
                "countryCode": "DE",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "rentalDays": 4,
              "segmentNumber": 5,
              "startDateTime": "2022-02-28T12:00:00Z",
              "vendorChainCode": "SX",
              "vendorChainName": "Sixt Rent a Car",
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
        },
        "hotel": {
          "id": "id6",
          "reservations": [
            {
              "address": {
                "address1": "Mahdentalstrasse 68.",
                "countryCode": "DE",
                "city": "Stuttgart",
                "postalCode": "71065",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "bookingDateTime": "bookingDateTime6",
              "checkInDateTime": "checkInDateTime0",
              "checkOutDateTime": "checkOutDateTime2",
              "confirmationNumber": "confirmationNumber0",
              "fare": {
                "amount": 50,
                "currencyCode": "currencyCode0",
                "description": "description0",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "guests": [
                {
                  "lastName": "NONAME FIRSTNAME",
                  "identifiers": [],
                  "exampleAdditionalProperty": {
                    "key1": "val1",
                    "key2": "val2"
                  }
                }
              ],
              "lineItems": [
                "lineItems0",
                "lineItems1"
              ],
              "numberOfNights": 74,
              "numberOfRooms": 248,
              "roomType": "roomType8",
              "segmentNumber": 154,
              "vendorChainCode": "vendorChainCode8",
              "vendorChainName": "vendorChainName2",
              "vendorCode": "vendorCode2",
              "vendorName": "vendorName4",
              "baseFare": {
                "amount": 2.42,
                "currencyCode": "currencyCode6",
                "description": "description4",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
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
        },
        "rail": {
          "id": "id0",
          "tickets": [
            {
              "legs": [
                {
                  "arrivalDateTime": "2022-02-28T12:08:00Z",
                  "arrivalStationCode": "ZWS",
                  "carrierCode": "LH",
                  "carrierName": "Lufthansa",
                  "departureDateTime": "2022-02-28T10:52:00Z",
                  "departureStationCode": "FRA",
                  "segmentNumber": 3,
                  "trainNumber": "3410",
                  "exampleAdditionalProperty": {
                    "key1": "val1",
                    "key2": "val2"
                  }
                }
              ],
              "recordLocator": "2CMDF7",
              "issueDateTime": "2022-01-06T17:03:00Z",
              "bookingDateTime": "2022-01-06T17:03:00Z",
              "fare": {
                "amount": 4574.77,
                "currencyCode": "USD",
                "description": "Total Fare",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "payments": [],
              "lineItems": [],
              "passenger": {
                "firstName": "FIRSTNAME",
                "lastName": "NONAME",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "isInternational": false,
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
        },
        "misc": {
          "id": "id8",
          "documents": [
            {
              "documentNumber": "8904804804804",
              "bookingType": "Purchase",
              "fare": {
                "amount": 10.77,
                "currencyCode": "USD",
                "description": "Total Fare",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "baseFare": {
                "amount": 10.77,
                "currencyCode": "USD",
                "description": "Base Fare"
              },
              "lineItems": [],
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
        },
        "exampleAdditionalProperty": {
          "key1": "val1",
          "key2": "val2"
        }
      },
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

