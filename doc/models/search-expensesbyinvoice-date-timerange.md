
# Search Expensesbyinvoice Date Timerange

*This model accepts additional fields of type unknown.*

## Structure

`SearchExpensesbyinvoiceDateTimerange`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `number` | Required | - |
| `status` | `string` | Required | - |
| `remainingRecords` | `number` | Required | - |
| `result` | [`Result1[]`](../../doc/models/result-1.md) | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "code": 46,
  "status": "status4",
  "remainingRecords": 12,
  "result": [
    {
      "id": "id6",
      "taxesTotal": 68.62,
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
          "productId": "1cc25604-13ef-0b36-3d5e-948f4a01e00d",
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
        },
        "car": {
          "id": "e5b0a390-5913-5a87-0d11-b6e148ca2da3",
          "reservations": [
            {
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "carType": "Intermediate Car Auto A/C",
              "confirmationNumber": "K03512717C2",
              "dropOffLocation": {
                "address1": "Hertz San Francisco International Airport",
                "address2": "780 McDonnell Road",
                "countryCode": "US",
                "city": "San Francisco",
                "region": "California",
                "postalCode": "94128",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "endDateTime": "2022-03-01T11:00:00Z",
              "isInternational": false,
              "lineItems": [],
              "numberOfCars": 1,
              "pickupLocation": {
                "address1": "Hertz San Francisco International Airport",
                "address2": "780 McDonnell Road",
                "countryCode": "US",
                "city": "San Francisco",
                "region": "California",
                "postalCode": "94128",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "rentalDays": 13,
              "segmentNumber": 5,
              "startDateTime": "2022-02-16T17:00:00Z",
              "vendorChainCode": "ZE",
              "vendorChainName": "Hertz Rent-A-Car",
              "exampleAdditionalProperty": {
                "key1": "val1",
                "key2": "val2"
              }
            },
            {
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "carType": "Intermediate Car Auto A/C",
              "confirmationNumber": "K0350953567",
              "dropOffLocation": {
                "address1": "Austin Bergstrom Intl Airport",
                "address2": "3819 Presidential Blvd",
                "countryCode": "US",
                "city": "Austin",
                "region": "Texas",
                "postalCode": "78719-2339",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "endDateTime": "2022-03-08T10:00:00Z",
              "isInternational": false,
              "lineItems": [],
              "numberOfCars": 1,
              "pickupLocation": {
                "address1": "Austin Bergstrom Intl Airport",
                "address2": "3819 Presidential Blvd",
                "countryCode": "US",
                "city": "Austin",
                "region": "Texas",
                "postalCode": "78719-2339",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "rentalDays": 7,
              "segmentNumber": 10,
              "startDateTime": "2022-03-01T18:45:00Z",
              "vendorChainCode": "ZE",
              "vendorChainName": "Hertz Rent-A-Car",
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
        "cruiseFerry": {
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
        },
        "hotel": {
          "id": "c15d8f3d-9371-f61d-a300-39f66c60e7a0",
          "reservations": [
            {
              "address": {
                "address1": "47000 Lakeview Blvd",
                "countryCode": "US",
                "city": "Fremont",
                "region": "California",
                "postalCode": "94538",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "checkInDateTime": "2022-02-15T15:00:00Z",
              "checkOutDateTime": "2022-03-01T11:00:00Z",
              "confirmationNumber": "91495930",
              "fare": {
                "amount": 1554,
                "currencyCode": "USD",
                "description": "Estimated Total",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "baseFare": {
                "amount": 78,
                "currencyCode": "USD",
                "description": "Daily",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "guests": [
                {
                  "lastName": "DOE JOHN MR",
                  "identifiers": [],
                  "exampleAdditionalProperty": {
                    "key1": "val1",
                    "key2": "val2"
                  }
                }
              ],
              "lineItems": [],
              "numberOfNights": 14,
              "numberOfRooms": 1,
              "roomType": "TED",
              "segmentNumber": 6,
              "vendorChainCode": "CY",
              "vendorChainName": "COURTYARD",
              "vendorCode": "17080",
              "vendorName": "Courtyard Fremont Marriott",
              "exampleAdditionalProperty": {
                "key1": "val1",
                "key2": "val2"
              }
            },
            {
              "address": {
                "address1": "304 E Cesar Chavez St",
                "countryCode": "US",
                "city": "Austin",
                "region": "Texas",
                "postalCode": "78701",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "checkInDateTime": "2022-03-01T15:00:00Z",
              "checkOutDateTime": "2022-03-08T11:00:00Z",
              "confirmationNumber": "90736911",
              "guests": [
                {
                  "lastName": "DOE JOHN MR",
                  "identifiers": [],
                  "exampleAdditionalProperty": {
                    "key1": "val1",
                    "key2": "val2"
                  }
                }
              ],
              "lineItems": [],
              "numberOfNights": 7,
              "numberOfRooms": 1,
              "roomType": "TED",
              "segmentNumber": 7,
              "vendorChainCode": "MC",
              "vendorChainName": "MARRIOTT",
              "vendorCode": "385152",
              "vendorName": "Austin Marriott Downtown",
              "fare": {
                "amount": 128,
                "currencyCode": "currencyCode0",
                "description": "description0",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "baseFare": {
                "amount": 242,
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
          "id": "035459ba-2bff-a68b-4576-034c86cbd76e",
          "tickets": [
            {
              "legs": [
                {
                  "arrivalDateTime": "2022-03-09T10:06:00Z",
                  "arrivalStationCode": "QDU",
                  "carrierCode": "LH",
                  "carrierName": "Lufthansa",
                  "classOfServiceCode": "S",
                  "departureDateTime": "2022-03-09T08:42:00Z",
                  "departureStationCode": "FRA",
                  "segmentNumber": 13,
                  "trainNumber": "3502",
                  "exampleAdditionalProperty": {
                    "key1": "val1",
                    "key2": "val2"
                  }
                }
              ],
              "recordLocator": "U7EKXS",
              "issueDateTime": "2022-02-11T09:19:00Z",
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "fare": {
                "amount": 942.07,
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
                "firstName": "JOHN",
                "lastName": "DOE",
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
        "tour": {
          "id": "01d02430-ee36-c268-96bb-5ed19122a45d",
          "reservations": [
            {
              "bookingDateTime": "2022-02-11T09:19:00Z",
              "carType": "LIMO",
              "confirmationNumber": "5831",
              "endDateTime": "2022-03-01T08:00:00Z",
              "endLocationAddress": {
                "address1": "EWR AIRPORT UA 2310",
                "address2": "EWR AIRPORT UA 2511",
                "countryCode": "AE",
                "city": "Dubai",
                "postalCode": "779944",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "fare": {
                "amount": 2,
                "currencyCode": "USD",
                "description": "Estimated Total"
              },
              "isInternational": false,
              "numberOfNights": 14,
              "numberOfRooms": 1,
              "segmentNumber": 9,
              "startDateTime": "2022-02-15T09:45:00Z",
              "startLocationAddress": {
                "address1": "14 COPE CT HILLSBOROUGH",
                "address2": "27 NOPE ST WILLSBOROUGH",
                "countryCode": "CE",
                "city": "LHR",
                "postalCode": "555444",
                "exampleAdditionalProperty": {
                  "key1": "val1",
                  "key2": "val2"
                }
              },
              "vendorChainName": "ADDISON",
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

