# Air-Fare-Search-Select-Seat

```ts
const airFareSearchSelectSeatApi = new AirFareSearchSelectSeatApi(client);
```

## Class Name

`AirFareSearchSelectSeatApi`

## Methods

* [Air Fare Rules](../../doc/controllers/air-fare-search-select-seat.md#air-fare-rules)
* [Air Seat Map](../../doc/controllers/air-fare-search-select-seat.md#air-seat-map)


# Air Fare Rules

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirFareRules(
  authorization: string,
  body: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | `string` | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body = '{\n	"api_key": "{{ASB_API_KEY}}",\n	"timestamp": "{{timestamp}}",\n	"nonce": "{{nonce}}",\n	"locale": "en_US",\n	"customer_ip": "127.0.0.1",\n	"session_id": "{{session_id}}",\n	"user_agent": "curl/7.64.0",\n	"system": "aft",\n	"configuration_id": {{configuration_id}},\n	"fare_group_key": "{{fare_group_key}}"\n}';

try {
  const response = await airFareSearchSelectSeatApi.mAirFareRules(
    authorization,
    body
  );

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


# Air Seat Map

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirSeatMap(
  authorization: string,
  body: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | `string` | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body = '{\n	"api_key": "{{ASB_API_KEY}}",\n	"timestamp": "{{timestamp}}",\n	"nonce": "{{nonce}}",\n	"locale": "en_US",\n	"customer_ip": "127.0.0.1",\n	"session_id": "{{session_id}}",\n	"user_agent": "curl/7.64.0",\n	"system": "aft",\n	\n	"configuration_id": {{configuration_id}},	\n	"fare_group_key": "{{fare_group_key}}",\n    "flight_option_keys": [\n        "{{flight_option_key_1}}"\n    ],\n	"traveler": {\n		"traveler_name": {\n			"first_name": "{{traveler_first_name}}",\n		    "last_name": "{{traveler_last_name}}"\n		}\n	}\n}';

try {
  const response = await airFareSearchSelectSeatApi.mAirSeatMap(
    authorization,
    body
  );

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

