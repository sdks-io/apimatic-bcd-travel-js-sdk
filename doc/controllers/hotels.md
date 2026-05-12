# Hotels

```ts
const hotelsController = new HotelsController(client);
```

## Class Name

`HotelsController`

## Methods

* [Get List](../../doc/controllers/hotels.md#get-list)
* [Get Detailed Info](../../doc/controllers/hotels.md#get-detailed-info)
* [Get Availability](../../doc/controllers/hotels.md#get-availability)
* [Get Rates](../../doc/controllers/hotels.md#get-rates)
* [Get Rate Details](../../doc/controllers/hotels.md#get-rate-details)
* [Get Recommended Rate](../../doc/controllers/hotels.md#get-recommended-rate)
* [Get Checkout Data](../../doc/controllers/hotels.md#get-checkout-data)
* [Book](../../doc/controllers/hotels.md#book)
* [Rebook](../../doc/controllers/hotels.md#rebook)
* [Cancel Reservation](../../doc/controllers/hotels.md#cancel-reservation)
* [Update Reservation Details](../../doc/controllers/hotels.md#update-reservation-details)
* [Get Reservations List](../../doc/controllers/hotels.md#get-reservations-list)
* [Get Reservation Details](../../doc/controllers/hotels.md#get-reservation-details)


# Get List

```ts
async getList(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  destination: string,
  chains: string,
  checkin: string,
  hotelNameKeyword: string,
  limit: number,
  order: string,
  page: number,
  searchRadius: number,
  searchRadiusUnit: string,
  starRatingFilter: string,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `destination` | `string` | Query, Required | - |
| `chains` | `string` | Query, Required | - |
| `checkin` | `string` | Query, Required | - |
| `hotelNameKeyword` | `string` | Query, Required | - |
| `limit` | `number` | Query, Required | - |
| `order` | `string` | Query, Required | - |
| `page` | `number` | Query, Required | - |
| `searchRadius` | `number` | Query, Required | - |
| `searchRadiusUnit` | `string` | Query, Required | - |
| `starRatingFilter` | `string` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const destination = 'Region:e|2786';

const chains = 'HH';

const checkin = '2023-07-11';

const hotelNameKeyword = 'Inn';

const limit = 10;

const order = 'name';

const page = 1;

const searchRadius = 5;

const searchRadiusUnit = 'KM';

const starRatingFilter = '4,4.5,5';

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getList(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    destination,
    chains,
    checkin,
    hotelNameKeyword,
    limit,
    order,
    page,
    searchRadius,
    searchRadiusUnit,
    starRatingFilter,
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


# Get Detailed Info

```ts
async getDetailedInfo(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  checkin: string,
  hotelId: number,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `checkin` | `string` | Query, Required | - |
| `hotelId` | `number` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const checkin = '2021-07-11';

const hotelId = 574889;

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getDetailedInfo(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    checkin,
    hotelId,
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


# Get Availability

```ts
async getAvailability(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  checkin: string,
  checkout: string,
  currency: string,
  guestCount: number,
  hotels: number,
  loyaltyProgramCodes: string,
  onlyAvailableHotels: boolean,
  returnPostpaidOnly: boolean,
  timeout: number,
  dontWaitForResults: boolean,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `checkin` | `string` | Query, Required | - |
| `checkout` | `string` | Query, Required | - |
| `currency` | `string` | Query, Required | - |
| `guestCount` | `number` | Query, Required | - |
| `hotels` | `number` | Query, Required | - |
| `loyaltyProgramCodes` | `string` | Query, Required | - |
| `onlyAvailableHotels` | `boolean` | Query, Required | - |
| `returnPostpaidOnly` | `boolean` | Query, Required | - |
| `timeout` | `number` | Query, Required | - |
| `dontWaitForResults` | `boolean` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const checkin = '2023-07-11';

const checkout = '2023-07-12';

const currency = 'EUR';

const guestCount = 1;

const hotels = 574889;

const loyaltyProgramCodes = 'Z99';

const onlyAvailableHotels = true;

const returnPostpaidOnly = false;

const timeout = 30;

const dontWaitForResults = false;

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getAvailability(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    checkin,
    checkout,
    currency,
    guestCount,
    hotels,
    loyaltyProgramCodes,
    onlyAvailableHotels,
    returnPostpaidOnly,
    timeout,
    dontWaitForResults,
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


# Get Rates

```ts
async getRates(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  checkin: string,
  checkout: string,
  currency: string,
  guestCount: number,
  hotelId: number,
  loyaltyProgramCodes: string,
  timeout: number,
  dateFormatType: string,
  dontWaitForResults: boolean,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `checkin` | `string` | Query, Required | - |
| `checkout` | `string` | Query, Required | - |
| `currency` | `string` | Query, Required | - |
| `guestCount` | `number` | Query, Required | - |
| `hotelId` | `number` | Query, Required | - |
| `loyaltyProgramCodes` | `string` | Query, Required | - |
| `timeout` | `number` | Query, Required | - |
| `dateFormatType` | `string` | Query, Required | - |
| `dontWaitForResults` | `boolean` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const checkin = '2021-07-11';

const checkout = '2021-07-12';

const currency = 'EUR';

const guestCount = 1;

const hotelId = 574889;

const loyaltyProgramCodes = 'Z99';

const timeout = 60;

const dateFormatType = 'fr';

const dontWaitForResults = false;

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getRates(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    checkin,
    checkout,
    currency,
    guestCount,
    hotelId,
    loyaltyProgramCodes,
    timeout,
    dateFormatType,
    dontWaitForResults,
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


# Get Rate Details

```ts
async getRateDetails(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  rateKey: string,
  guestCount: number,
  hotelId: number,
  dateFormatType: string,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `rateKey` | `string` | Query, Required | - |
| `guestCount` | `number` | Query, Required | - |
| `hotelId` | `number` | Query, Required | - |
| `dateFormatType` | `string` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const rateKey = 'eJxNTEtuwjAU3HOKd4AE7Edw3Nk58QNbhMRKUoTYIcGCql213L8JYsEsRqP5sWLOlc3XatQbaAM2S2W5KC1QAJuysPYDCAFP7IDLz+V6e/zOXgqNmVboXQ04xc3RAJXeA6xY56rMtX7TPIXWZ1Xw2VZ8Nq2ys3kefw7+RczFUuGFr8f3/fYHbBs5xaoR6t0oC0372O6oEr+ou0OiEGlIIp5iO0rfykgrcilN9Zjc7FLfdYd/eLc5NQ==';

const guestCount = 1;

const hotelId = 574889;

const dateFormatType = 'fr';

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getRateDetails(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    rateKey,
    guestCount,
    hotelId,
    dateFormatType,
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


# Get Recommended Rate

```ts
async getRecommendedRate(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  rateKey: string,
  guestCount: number,
  hotelId: number,
  dateFormatType: string,
  searchId: string,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `rateKey` | `string` | Query, Required | - |
| `guestCount` | `number` | Query, Required | - |
| `hotelId` | `number` | Query, Required | - |
| `dateFormatType` | `string` | Query, Required | - |
| `searchId` | `string` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const rateKey = 'eJxNTEtuwjAU3HOKd4AE7Edw3Nk58QNbhMRKUoTYIcGCql213L8JYsEsRqP5sWLOlc3XatQbaAM2S2W5KC1QAJuysPYDCAFP7IDLz+V6e/zOXgqNmVboXQ04xc3RAJXeA6xY56rMtX7TPIXWZ1Xw2VZ8Nq2ys3kefw7+RczFUuGFr8f3/fYHbBs5xaoR6t0oC0372O6oEr+ou0OiEGlIIp5iO0rfykgrcilN9Zjc7FLfdYd/eLc5NQ==';

const guestCount = 1;

const hotelId = 574889;

const dateFormatType = 'fr';

const searchId = '68lkU9QBGOmOLdrI2hlaSl';

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getRecommendedRate(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    rateKey,
    guestCount,
    hotelId,
    dateFormatType,
    searchId,
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


# Get Checkout Data

```ts
async getCheckoutData(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  acceptedCreditCards: string,
  checkout: string,
  internalTravelerId: number,
  paidPolicy: string,
  tspmCompanyId: number,
  tspmTravelerId: number,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `acceptedCreditCards` | `string` | Query, Required | - |
| `checkout` | `string` | Query, Required | - |
| `internalTravelerId` | `number` | Query, Required | - |
| `paidPolicy` | `string` | Query, Required | - |
| `tspmCompanyId` | `number` | Query, Required | - |
| `tspmTravelerId` | `number` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const acceptedCreditCards = 'VI,MC';

const checkout = '2021-07-12';

const internalTravelerId = 123;

const paidPolicy = 'D';

const tspmCompanyId = 20.001;

const tspmTravelerId = 24.001;

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getCheckoutData(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    acceptedCreditCards,
    checkout,
    internalTravelerId,
    paidPolicy,
    tspmCompanyId,
    tspmTravelerId,
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


# Book

```ts
async book(
  authorization: string,
  body: Hotelsbookrequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`Hotelsbookrequest`](../../doc/models/hotelsbookrequest.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: Hotelsbookrequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  configurationId: 4,
  system: 'aft',
  booktrackId: '{{timestamp}}',
  guestCount: 1,
  hotelId: 574889,
  originalCurrency: 'USD',
  originalTotal: 229.15,
  rateKey: 'eJxNjM0SwUAQhO+eYh5A2Bn5WX0bdsumkGwloYqbKg4UJ7y/hIs+dX/d1WJEEmOTGXeGIRmyfJKKFbZACmRFau0cCAFfrYDT43S+vJ8Di2GTcwbEpgbUiJo+LHgNiBFOTJEw/3npy+DG/Xp8zL+HftcAu9YBPC8mw+Cn2/t+vbz6T1VqOz2QVo5a3fsR07qsVrTwbrSst5FCSW303lFZdb6pfEdT0hg3nsqoA6WmrrcfzNk4Wg==',
  bookerEmail: 'booker@bcdtriptech.com',
  bookerFirstName: 'BookerFirst',
  bookerLastName: 'BookerLast',
  travelerEmail: 'traveler@bcdtriptech.com',
  travelerFirstName: 'TravelerFirst',
  travelerLastName: 'TravelerLast',
  paymentMethod: 'card',
  loyaltyCardChainCode: 'RT',
  loyaltyCardNumber: '1001709',
  creditCardNumber: '5555555555554444',
  creditCardExpirationYear: '2030',
  creditCardExpirationMonth: '01',
  creditCardFirstName: 'GHOST',
  creditCardLastName: 'CARD',
  creditCardAddress: 'addr1',
  creditCardCountryCode: 'US',
  creditCardCity: 'Atlanta',
  creditCardStateProvinceCode: 'GA',
  creditCardPostalCode: '12345',
  creditCardPhone: '1234567890',
};

try {
  const response = await hotelsController.book(
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


# Rebook

```ts
async rebook(
  authorization: string,
  body: Hotelsrebookrequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`Hotelsrebookrequest`](../../doc/models/hotelsrebookrequest.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: Hotelsrebookrequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  bookingUid: 'dc2ee73lfjykj4zliaqlm5xix',
  booktrackId: '{{timestamp}}',
  hotelId: 574889,
  originalCurrency: 'USD',
  originalTotal: 229.15,
  rateKey: 'eJxNjMtOwzAURPf9ivsBTWubvDq768SKrSaxFTtFsKtEFyBYQf8fp2yY1TyORgmlCtEWTzIJCVWhqg+lapVsgRKomrJtT4C1eGgArl/Xt9v9e+uCHWtZAWHxAIuSRQ6DPANKKFmIppDyn1eAtv0+0/vX+nFo1gVYYw/IU3PYgD993D/fbz/5k5li4hfiuafIF7OTdHbzQJPXbnQpD11nYnR6NPR8JM3JplXvOj8Fso5iMKYnNyezzCbRkTiETLrAW0uL99MvQXY/vQ==',
  bookerEmail: 'booker@bcdtriptech.com',
  bookerFirstName: 'BookerFirst',
  bookerLastName: 'BookerLast',
};

try {
  const response = await hotelsController.rebook(
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


# Cancel Reservation

```ts
async cancelReservation(
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
  email: 'booker@bcdtriptech.com',
  bookingUid: 'c45ku73jdbjlczjktkdzanpcmi',
};

try {
  const response = await hotelsController.cancelReservation(
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


# Update Reservation Details

```ts
async updateReservationDetails(
  authorization: string,
  body: HotelsupdateReservationDetailsRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`HotelsupdateReservationDetailsRequest`](../../doc/models/hotelsupdate-reservation-details-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: HotelsupdateReservationDetailsRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  bookingUid: 'dc2ee73lfjykj4zliaqlm5xix',
  bookingData: {
    isGhost: false,
  },
};

try {
  const response = await hotelsController.updateReservationDetails(
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


# Get Reservations List

```ts
async getReservationsList(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  configurationId: number,
  system: string,
  travelerEmail: string,
  status: string,
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
| `configurationId` | `number` | Query, Required | - |
| `system` | `string` | Query, Required | - |
| `travelerEmail` | `string` | Query, Required | - |
| `status` | `string` | Query, Required | - |
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

const configurationId = 4;

const system = 'aft';

const travelerEmail = 'traveler@bcdtriptech.com';

const status = 'canceled';

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getReservationsList(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    configurationId,
    system,
    travelerEmail,
    status,
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


# Get Reservation Details

```ts
async getReservationDetails(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  travelerEmail: string,
  bookingUid: string,
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
| `travelerEmail` | `string` | Query, Required | - |
| `bookingUid` | `string` | Query, Required | - |
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

const travelerEmail = 'traveler@bcdtriptech.com';

const bookingUid = 'c45ku73jdbjlczjktkdzanpcmi';

const authorization = 'Signature {{signature}}';

try {
  const response = await hotelsController.getReservationDetails(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    travelerEmail,
    bookingUid,
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

