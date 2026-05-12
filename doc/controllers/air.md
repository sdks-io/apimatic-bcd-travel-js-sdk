# Air

```ts
const airApi = new AirApi(client);
```

## Class Name

`AirApi`

## Methods

* [Air Destination Lookup ? Api Key ASB API KEY Timestamp Timestamp Nonce Nonce Locale En US Customer Ip 127 0 0 1 Session Id Session Id User Agent Curl 7 64 0 System Aft Configuration Id 4 Term Irpin](../../doc/controllers/air.md#air-destination-lookup-api-key-asb-api-key-timestamp-timestamp-nonce-nonce-locale-en-us-customer-ip-127-0-0-1-session-id-session-id-user-agent-curl-7-64-0-system-aft-configuration-id-4-term-irpin)
* [Air Documents Issue](../../doc/controllers/air.md#air-documents-issue)
* [Air Complete Verification](../../doc/controllers/air.md#air-complete-verification)
* [Air Retrieve Reservations List](../../doc/controllers/air.md#air-retrieve-reservations-list)


# Air Destination Lookup ? Api Key ASB API KEY Timestamp Timestamp Nonce Nonce Locale En US Customer Ip 127 0 0 1 Session Id Session Id User Agent Curl 7 64 0 System Aft Configuration Id 4 Term Irpin

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirDestinationLookupApiKeyAsbApiKeyTimestampTimestampNonceNonceLocaleEnUsCustomerIp127001SessionIdSessionIdUserAgentCurl7640SystemAftConfigurationId4TermIrpin(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  term: string,
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
| `term` | `string` | Query, Required | - |
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

const term = 'lond';

const authorization = 'Signature {{signature}}';

try {
  const response = await airApi.mAirDestinationLookupApiKeyAsbApiKeyTimestampTimestampNonceNonceLocaleEnUsCustomerIp127001SessionIdSessionIdUserAgentCurl7640SystemAftConfigurationId4TermIrpin(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    term,
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


# Air Documents Issue

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirDocumentsIssue(
  authorization: string,
  body: AirdocumentsIssueRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`AirdocumentsIssueRequest`](../../doc/models/airdocuments-issue-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: AirdocumentsIssueRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  bookingUid: '63a36d2c2d4d55f488e097c2',
  issueTickets: true,
  issueEmds: true,
};

try {
  const response = await airApi.mAirDocumentsIssue(
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


# Air Complete Verification

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirCompleteVerification(
  authorization: string,
  body: AircompleteVerificationRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`AircompleteVerificationRequest`](../../doc/models/aircomplete-verification-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: AircompleteVerificationRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  verificationId: 'SdclrQ5x8BumYVOXbwmJ5tIYKNG5sUe0unafapdxpasdRfbFdjM40g==',
};

try {
  const response = await airApi.mAirCompleteVerification(
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


# Air Retrieve Reservations List

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirRetrieveReservationsList(
  authorization: string,
  body: AirretrieveReservationsListRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`AirretrieveReservationsListRequest`](../../doc/models/airretrieve-reservations-list-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: AirretrieveReservationsListRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  travelerEmail: 'rkaydanowski+hcat@bcdtriptech.com',
  limit: 10,
  offset: 11,
  currency: 'UAH',
};

try {
  const response = await airApi.mAirRetrieveReservationsList(
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

