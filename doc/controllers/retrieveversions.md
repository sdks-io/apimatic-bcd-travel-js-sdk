# Retrieveversions

```ts
const retrieveversionsApi = new RetrieveversionsApi(client);
```

## Class Name

`RetrieveversionsApi`


# Get Versionsbytrip Id

The Retrieve Expense Versions Request will return versions of an expense item by its trip identifier. Request is configured via URL link only. Filters are not supported by this API.

> **tripId -** A unique identifier of an Expense in BCD (guid).

```ts
async getVersionsbytripId(
  tripId: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<GetVersionsbytripId>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `tripId` | `string` | Template, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance. The `result` property of this instance returns the response data which is of type [`GetVersionsbytripId`](../../doc/models/get-versionsbytrip-id.md).

## Example Usage

```ts
const tripId = '3c5100a0-4fbb-1225-a41a-86a928031db7';

try {
  const response = await retrieveVersionsApi.getVersionsbytripId(tripId);

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

