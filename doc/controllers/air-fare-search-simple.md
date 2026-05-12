# Air-Fare-Search-Simple

```ts
const airFareSearchSimpleApi = new AirFareSearchSimpleApi(client);
```

## Class Name

`AirFareSearchSimpleApi`

## Methods

* [Init](../../doc/controllers/air-fare-search-simple.md#init)
* [Air Fare Search](../../doc/controllers/air-fare-search-simple.md#air-fare-search)
* [Air Pricing](../../doc/controllers/air-fare-search-simple.md#air-pricing)
* [Air Book](../../doc/controllers/air-fare-search-simple.md#air-book)
* [Wait 10 Seconds](../../doc/controllers/air-fare-search-simple.md#wait-10-seconds)
* [Air Get Reservation Details](../../doc/controllers/air-fare-search-simple.md#air-get-reservation-details)
* [Air Cancel Reservation](../../doc/controllers/air-fare-search-simple.md#air-cancel-reservation)


# Init

:information_source: **Note** This endpoint does not require authentication.

```ts
async init(
  authorization: string,
  contentType: ContentType,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `contentType` | [`ContentType`](../../doc/models/content-type.md) | Header, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const contentType = ContentType.EnumApplicationjson;

try {
  const response = await airFareSearchSimpleApi.init(
    authorization,
    contentType
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


# Air Fare Search

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirFareSearch(
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

const body = '{\n    "api_key": "{{ASB_API_KEY}}",\n    "timestamp": "{{timestamp}}",\n    "nonce": "{{nonce}}",\n    "locale": "en_US",\n    "customer_ip": "127.0.0.1",\n    "session_id": "{{session_id}}",\n    "user_agent": "curl/7.64.0",\n    "system": "aft",\n    "configuration_id": {{configuration_id}},\n    "currency": "{{currency}}",\n    "travelers": [\n        {\n            "traveler_type": "{{traveler_type}}"\n        }\n    ],\n    "origin_destinations": [\n        {\n            "departure_location": {\n                "location_code": "{{departure_1}}",\n                "location_type": "airport"\n            },\n            "arrival_location": {\n                "location_code": "{{arrival_1}}",\n                "location_type": "airport"\n            },\n            "direct_only": {{direct_only}},\n            "departure_date": "{{departure_date_1}}"\n        }\n    ],\n    "included_baggage": false,\n    "refundable_only": false,\n    "changeable_only": false,\n    "exclude_penalties": false\n}';

try {
  const response = await airFareSearchSimpleApi.mAirFareSearch(
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


# Air Pricing

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirPricing(
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

const body = '{\n    "api_key": "{{ASB_API_KEY}}",\n    "timestamp": "{{timestamp}}",\n    "nonce": "{{nonce}}",\n    "locale": "en_US",\n    "customer_ip": "127.0.0.1",\n    "session_id": "{{session_id}}",\n    "user_agent": "curl/7.64.0",\n    "system": "aft",\n    "configuration_id": {{configuration_id}},\n    "currency": "{{currency}}",\n    "fare_group_key": "{{fare_group_key}}",\n    "flight_option_keys": [\n        "{{flight_option_key_1}}"\n    ],\n    "travelers": [\n        {\n            "traveler_type": "{{traveler_type}}"\n        }\n    ]\n}';

try {
  const response = await airFareSearchSimpleApi.mAirPricing(
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


# Air Book

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirBook(
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

const body = '{\n    "api_key": "{{ASB_API_KEY}}",\n    "timestamp": "{{timestamp}}",\n    "nonce": "{{nonce}}",\n    "locale": "en_US",\n    "customer_ip": "127.0.0.1",\n    "session_id": "{{session_id}}",\n    "user_agent": "curl/7.64.0",\n    "configuration_id": {{configuration_id}},\n    "system": "aft",\n    \n    "booktrack_id": "{{timestamp}}",\n    \n    "fare_group_key": "{{fare_group_key}}",\n    "flight_option_keys": ["{{flight_option_key_1}}"],\n    "booker_email": "{{BOOKER_EMAIL}}",\n    "booker_first_name": "{{booker_first_name}}",\n    "booker_last_name": "{{booker_last_name}}",\n    \n    "payment_method": "{{payment_method}}",\n    \n    "credit_card_number": "{{credit_card_number}}",\n    "credit_card_expiration_year": "{{credit_card_expiration_year}}",\n    "credit_card_expiration_month": "{{credit_card_expiration_month}}",\n    "credit_card_first_name": "{{credit_card_first_name}}",\n    "credit_card_last_name": "{{credit_card_last_name}}",\n    "credit_card_identifier": "{{credit_card_identifier}}",\n    \n    "billing_address": {\n        "city": "{{billing_address_city}}",\n        "country_code": "{{billing_address_country_code}}",\n        "postal_code": "{{billing_address_postal_code}}",\n        "state_code": "{{billing_address_state_code}}",\n        "street_address1": "{{billing_address_street_address}}"\n    },\n    \n    "phone_number": "{{traveler_phone_number}}",\n    \n    "travelers": [\n        {\n        	"date_of_birth": "{{traveler_date_of_birth}}",\n            "gender": "{{traveler_gender}}",\n            "traveler_email": "{{traveler_email}}",\n            "traveler_name": {\n            	"first_name": "{{traveler_first_name}}",\n            	"last_name": "{{traveler_last_name}}"\n            },\n            "passport": {\n				"country_of_issue": "{{passport_country_of_issue}}",\n				"expiry_date": "{{passport_expiry_date}}",\n				"nationality": "{{passport_nationality}}",\n				"number": "{{passport_number}}"\n            },\n            "tspm_traveler_id": "{{tspm_traveler_id}}"\n        }\n    ],\n    \n    "tspm_company_id": "{{tspm_company_id}}"\n}';

try {
  const response = await airFareSearchSimpleApi.mAirBook(
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


# Wait 10 Seconds

:information_source: **Note** This endpoint does not require authentication.

```ts
async wait10Seconds(
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
try {
  const response = await airFareSearchSimpleApi.wait10Seconds();

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


# Air Get Reservation Details

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirGetReservationDetails(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  bookingUid: string,
  currency: string,
  authorization: string,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `apiKey` | `string` | Query, Required | - |
| `timestamp` | `string` | Query, Required | - |
| `nonce` | `string` | Query, Required | - |
| `locale` | `string` | Query, Required | - |
| `customerIp` | `string` | Query, Required | - |
| `sessionId` | `string` | Query, Required | - |
| `userAgent` | `string` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `bookingUid` | `string` | Query, Required | - |
| `currency` | `string` | Query, Required | - |
| `authorization` | `string` | Header, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const apiKey = '{{ASB_API_KEY}}';

const timestamp = '{{timestamp}}';

const nonce = '{{nonce}}';

const locale = 'en_US';

const customerIp = '127.0.0.1';

const sessionId = '{{session_id}}';

const userAgent = 'curl/7.64.0';

const system = 'aft';

const bookingUid = '{{booking_uid}}';

const currency = 'UAH';

const authorization = 'Signature {{signature}}';

try {
  const response = await airFareSearchSimpleApi.mAirGetReservationDetails(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    bookingUid,
    currency,
    authorization
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


# Air Cancel Reservation

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirCancelReservation(
  authorization: string,
  body: HotelscancelReservationRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`HotelscancelReservationRequest`](../../doc/models/hotelscancel-reservation-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: HotelscancelReservationRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  email: '{{BOOKER_EMAIL}}',
  bookingUid: '{{booking_uid}}',
};

try {
  const response = await airFareSearchSimpleApi.mAirCancelReservation(
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

