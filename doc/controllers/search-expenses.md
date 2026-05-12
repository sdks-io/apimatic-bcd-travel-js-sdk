# Search Expenses

```ts
const searchExpensesApi = new SearchExpensesApi(client);
```

## Class Name

`SearchExpensesApi`


# Search Expenses

The Search Expenses Request will return a list of expenses that match the requested search criteria. API allows pagination by using limit (number of results on the page) and offset values (next batch of items to return starting from the offset).

> **limit -** The maximum number of records to return on this particular call. If a user has 45 records but 'limit' is set to 20 and offset is not set, the first 20 records out of the 45 will be returned. If 'offset' is set to 21, this will return the next 20 results (#21-40). If 'offset' is set to 41 and 'limit' is still 20, we will receive the last few results in the total list (#41-45). Valid values can be between 1 and 100.

> **offset** - The n'th record in the total list from which the results in this call will start. If a user has 45 records, but this 'limit' is set to 20 and 'offset' is not set, the first 20 records out of the 45 will be returned. If offset is set to 21, this will return the next 20 results (#21-40). If 'offset' is set to 41 and 'limit' is still 20, we will receive the last few results in the total list (#41-45). Minimum value of offset is 0.

Filters:

> **recordLocator** - The GDS passenger name record (PNR) identifier. Specify single or multiple values.

> **invoiceNumber -** The invoice number from the vendor for the invoice. Specify single or multiple values.

> **travelerEmail** - The traveler email address associated with the trip record. Specify single or multiple values.

> **bookingDateTime** - The ISO 8601 date/time when the booking was created. Note: the date (in YYYY-MM-DD format) is required. Only hours and minutes (not seconds) can be specified in the request. Examples: for ranges: 2020-02-14T19:47 TO 2020-02-18T19:47, for single date: 2020-02-14T19:47.

> **invoiceDateTime** - The ISO 8601 date/time or date/time range of the invoice issue. Our systems search any expense items with issue date that falls on or within the specified date/time range. Note: the date (in YYYY-MM-DD format) is required. Only hours and minutes (not seconds) can be specified in the request. Examples: for ranges: 2020-02-14T19:47 TO 2020-02-18T19:47, for single date: 2020-02-14T19:47.

> **lastModifiedDateTime** - The ISO 8601 date/time or date/time range when the booking was last modified. Note: the date (in YYYY-MM-DD format) is required. Only hours and minutes (not seconds) can be specified in the request. Examples: for ranges: 2020-02-14T19:47 TO 2020-02-18T19:47, for single date: 2020-02-14T19:47.

> **accountId** - The BCD specific identifier for the regional corporate office that owns the record (aka SMID). Specify single or multiple values.

> **globalCustomerNumber** - The global BCD specific number of the corporate account (in 'accountId'). Specify single or multiple values.

> **customerNumber** - The back office customer number associated with the customer name. Specify single or multiple values.

> **hasTransaction** - True if response should only return expense items with transactions, i.e. containing at least one air or rail ticket.

> **ticketStatus** - Ticket status in GDS. This filter is case insensitive.

> **calculatedTicketStatus** - Ticket status calculated based on the combination of coupon statuses. This filter is case insensitive.

Sort:

> **lastModifiedDateTime** - Sort by date/time when the booking was last modified. Specify the order you wish the data to be listed in: 'asc' or 'desc'.

> **invoiceDateTime** - Sort by date/time of the invoice issue. Specify the order you wish the data to be listed in: 'asc' or 'desc'.

```ts
async searchExpenses(
  body: SearchExpensesRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<SearchExpenses>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`SearchExpensesRequest`](../../doc/models/search-expenses-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`SearchExpenses`](../../doc/models/search-expenses.md).

## Example Usage

```ts
const body: SearchExpensesRequest = {
  limit: 50,
  offset: 0,
  filter: {
    invoiceNumber: [
      '850176',
      '850177'
    ],
    travelerEmail: [
      'FIRSTNAME.NONAME@COMPANY.COM',
      'JDOE@SOMEWHERE.COM'
    ],
    bookingDateTime: '2022-01-01T00:01 TO 2022-02-17T00:01',
    invoiceDateTime: '2022-01-01T00:01 TO 2022-02-17T00:01',
    lastModifiedDateTime: '2022-01-01T00:01 TO 2022-02-17T00:01',
    customerNumber: [
      '9999999999',
      '9999999'
    ],
    accountId: [
      '999999901',
      '999999902'
    ],
    globalCustomerNumber: [
      '9999',
      '20109999'
    ],
    hasTransaction: true,
    recordLocator: [
      'GKQLV1',
      'EKDCAG'
    ],
    ticketStatus: [
      'TICKETED'
    ],
    calculatedTicketStatus: [
      'USED/FLOWN'
    ],
  },
  sort: {
    lastModifiedDateTime: 'asc',
    invoiceDateTime: 'desc',
  },
};

try {
  const response = await searchExpensesApi.searchExpenses(body);

  // Extracting fully parsed response body.
  console.log(response.result);

  // Extracting response status code.
  console.log(response.statusCode);
  // Extracting response headers.
  console.log(response.headers);
  // Extracting response body of type `string | Stream`
  console.log(response.body);
} catch (error) {
  if (error instanceof ApiError) {
    // Extracting response error status code.
    console.log(error.statusCode);
    // Extracting response error headers.
    console.log(error.headers);
    // Extracting response error body of type `string | Stream`.
    console.log(error.body);
  }
}
```

