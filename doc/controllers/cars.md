# Cars

```ts
const carsApi = new CarsApi(client);
```

## Class Name

`CarsApi`

## Methods

* [Cars Get Availability](../../doc/controllers/cars.md#cars-get-availability)
* [Cars Get Rate Details](../../doc/controllers/cars.md#cars-get-rate-details)
* [Cars Get Checkout Data](../../doc/controllers/cars.md#cars-get-checkout-data)
* [Cars Get Direct Sell Checkout Data](../../doc/controllers/cars.md#cars-get-direct-sell-checkout-data)
* [Cars Book Card](../../doc/controllers/cars.md#cars-book-card)
* [Cars Modify Reservation](../../doc/controllers/cars.md#cars-modify-reservation)
* [Cars Direct Sell Book No Payment](../../doc/controllers/cars.md#cars-direct-sell-book-no-payment)
* [Cars Cancel Reservation](../../doc/controllers/cars.md#cars-cancel-reservation)
* [Cars Get Reservations List](../../doc/controllers/cars.md#cars-get-reservations-list)
* [Cars Retrieve Reservations List](../../doc/controllers/cars.md#cars-retrieve-reservations-list)
* [Cars Get Reservation Details](../../doc/controllers/cars.md#cars-get-reservation-details)


# Cars Get Availability

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetAvailability(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  configurationId: number,
  currency: string,
  pickupLocation: string,
  pickupDatetime: string,
  dropoffDatetime: string,
  searchRadiusUnit: string,
  idNumbers: string,
  cdNumbers: string,
  carTypes: string,
  vendorCodes: string,
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
| `configurationId` | `number` | Query, Required | - |
| `currency` | `string` | Query, Required | - |
| `pickupLocation` | `string` | Query, Required | - |
| `pickupDatetime` | `string` | Query, Required | - |
| `dropoffDatetime` | `string` | Query, Required | - |
| `searchRadiusUnit` | `string` | Query, Required | - |
| `idNumbers` | `string` | Query, Required | - |
| `cdNumbers` | `string` | Query, Required | - |
| `carTypes` | `string` | Query, Required | - |
| `vendorCodes` | `string` | Query, Required | - |
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

const configurationId = 4;

const currency = 'EUR';

const pickupLocation = 'LHR';

const pickupDatetime = '2023-09-11T10:00';

const dropoffDatetime = '2023-09-12T10:00';

const searchRadiusUnit = 'KM';

const idNumbers = 'EP:40184175';

const cdNumbers = 'EP:40125456';

const carTypes = 'EBAR,ECMR,EDAR';

const vendorCodes = 'EP';

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetAvailability(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    configurationId,
    currency,
    pickupLocation,
    pickupDatetime,
    dropoffDatetime,
    searchRadiusUnit,
    idNumbers,
    cdNumbers,
    carTypes,
    vendorCodes,
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


# Cars Get Rate Details

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetRateDetails(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  configurationId: number,
  rateKey: string,
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
| `configurationId` | `number` | Query, Required | - |
| `rateKey` | `string` | Query, Required | - |
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

const configurationId = 4;

const rateKey = 'UWXSTXYeT7BVaZ4AsALgoh23kPmKFhANqGURgd_5dj04315AyfgFcCHFdWUVd4MQZpbIF1glSl_UnLPMiGIDJw97UeZUuAO1G4sH1VYFY2sKlAbhQ6d-HXNtq_BnuhISksspXrPehB4kf3Bz3hyl5z4vmqyBzmOTigZ_Lbjnf9fbid9t-m0HiyERV5Nvrjm_bHDYFZqeXpd_gbBgP_HVsU0o7OicGYltoGebP2IoxtSTVtWMz-wlbVK8enxn3dcvOH7LtEPKm6i1ITHbtlpUkuhohyok7_22j2DS2hpbq_kvr9TdEHavm2eWyP0fUnjwNRiLztV3Z__PKHB85n9fqm57tKekcW2zrFTvbAq1pHamuIVqchfVt0YAhnShENADPHN_9hufsCehwB60aqkDrhU8oCAWRG_0VdtQ81_oJ97MwCpoDKrqPtNumSukcPZLIZYVUF2_Imq3K_PmX_P3AIF4YBOJu1MMcD2p_DVnhV0P2CyIfo7QlxHA9LvW_I9gaSEusJXvOyrcPxcFLLSzpBk3-luJvQh4JtXXGqlf9ATkdDvenQ9uDFl9GSW5lME46vR3Ny8tuogU4LURou87qrPrcWs4cF4qjIFVlafPY5j85q13zVsxxdslSJMMCnbmbqNlgOc3toxkDsq0JIszGYp0ERoios4cUuCDaq0wtPasFwyEVp9gg1A=';

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetRateDetails(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    configurationId,
    rateKey,
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


# Cars Get Checkout Data

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetCheckoutData(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  configurationId: number,
  rateKey: string,
  internalTravelerId: number,
  tspmTravelerId: number,
  tspmCompanyId: number,
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
| `configurationId` | `number` | Query, Required | - |
| `rateKey` | `string` | Query, Required | - |
| `internalTravelerId` | `number` | Query, Required | - |
| `tspmTravelerId` | `number` | Query, Required | - |
| `tspmCompanyId` | `number` | Query, Required | - |
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

const configurationId = 4;

const rateKey = 'GIL2kt_ghfzs8mQzY8rjS8r7DmceUSwjBFcWMGrz5JZTmaM5DxY5015eal6eSH1BwNsB6HcDeaOXbJG3AQi6iFZNVDiTUb6AgX_uyre_ZodUCGl532oZ_IZejUpa7DbzdKfarMIw63iy1RHh4jKvXE4i79MMSFNYWEqOMBcPUC8Ls9Nd_nrkmISngzmpiDP_YLVZsMQvWc_nRd0IXWTxDdPMXkECym7pUgvZ0jtJ2FaU6jC1qF4nR9zQVnw3JM-25SxrONA9oTb0ivwfNZ5JJ9uUrrzwZNlsO40dTDiIP0GYPOuoZRi17ZxHxp_uu-rcEhbx83UWlGeR62LWGVQnpfpcvPEsNgOve5mXrE2iNwfJaTZCbxWB9ZP9VMMgiTL03AnGGGhoojFiywuu2P0zkDuVl4sS9UNl9Ub3Nqs6l1HoXCr8BdVfq4V2c-bt6pW_vtkKEsgl7fJcoQsdMH-m-lUq5CvOTSA4GeLh733METeXH2MKY-xBYLqLKvtsR_OSBGGhUUbFr0WaHVca2kojnbazVwI0aP6ood4h451wWE4oMcp91WE3slvKOqrA2TENTNLle22jdtQbjyHahHe96qhADWi8h0ewQtT1MjcbYomZ7Ix52doe_0ZxPwiyW7fX5c0xnAqJLUY-dU6uKs2EuUCHWU9UrmE_LHwrYU0RW8z3wYVkwo4AHBQ=';

const internalTravelerId = 123;

const tspmTravelerId = 24.001;

const tspmCompanyId = 20.001;

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetCheckoutData(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    configurationId,
    rateKey,
    internalTravelerId,
    tspmTravelerId,
    tspmCompanyId,
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


# Cars Get Direct Sell Checkout Data

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetDirectSellCheckoutData(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
  configurationId: number,
  tspmTravelerId: number,
  tspmCompanyId: number,
  vendorCode: string,
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
| `configurationId` | `number` | Query, Required | - |
| `tspmTravelerId` | `number` | Query, Required | - |
| `tspmCompanyId` | `number` | Query, Required | - |
| `vendorCode` | `string` | Query, Required | - |
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

const configurationId = 4;

const tspmTravelerId = 24.001;

const tspmCompanyId = 20.001;

const vendorCode = 'EP';

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetDirectSellCheckoutData(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
    configurationId,
    tspmTravelerId,
    tspmCompanyId,
    vendorCode,
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


# Cars Book Card

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsBookCard(
  authorization: string,
  body: Carsbookcardrequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`Carsbookcardrequest`](../../doc/models/carsbookcardrequest.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: Carsbookcardrequest = {
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
  rateKey: 'HXTA-wctTtPdSwR0YwTgxf-sQC0HtnMUY1LzJK9VGCdQejcoM_APOabKwHM6imiVD9poTZnXqc_fCWoi879kxynYmjEJ4Gmxy07E4lOfYJ5JJiunbu1l3SiNnbmADGS5WO4DhWZhMu6uIvkWf1zRsQ9twRN5z4_KrWKQJTCjMvQCNnY05OuSXKEldTrJSW-Ge2cqDE8DRAf-f3keu9jxwLy8KGihqmY1_zTAaaPHyOqRQnA88a2laCR8k7SmcMdzMdzB_h7OJqsF0opsrM3x_g6oN54-s9DJXLe0ohbrdNsgscJd0s2EzurxHNFgh2M8taFPJE4WEjBBK0qJqVXovnVCE0UXYJDdKXUYmnBmm2o9t_MMtNkfYPrWZF2vJQC-NNiWqqDa9kKm9jTeQxbnQH0qOaAkDlASm08aFsa_Bq-NZTLcKKUtxENAXSe1pP2p2OK3vwmN0jgLnIocWHXHQMT1Tov7X0dhv1Qd-yK5d__gi6v6tcv2pREKYg_RABmzsvEc7Qk6e-HDm-A-Vs5xZaLuD2O49_4kaE7t2UbiXezGw8h8g4Wg0GL3kpPFTrbNBwqBh_mCUCoGk-dRDs3XSiVtLv9GhkvF8C7MLL0nvKOORdi8hCyabkda79vj0wPUJnzMI7jebOR7p2TKRRnaKYC4bS8PCOusNEGxw276XUne0mkapAe3ziw=',
  bookerEmail: 'booker@bcdtriptech.com',
  bookerFirstName: 'BookerFirst',
  bookerLastName: 'BookerLast',
  pnrId: 'NQ86M3',
  travelerEmail: 'traveler@bcdtriptech.com',
  travelerFirstName: 'TravelerFirst',
  travelerLastName: 'TravelerLast',
  specialInformation: 'some spec info',
  paymentMethod: 'card',
  creditCardNumber: '4111111111111111',
  creditCardExpirationYear: '2020',
  creditCardExpirationMonth: '12',
  creditCardFirstName: 'CCFirst',
  creditCardLastName: 'CCLast',
};

try {
  const response = await carsApi.mCarsBookCard(
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


# Cars Modify Reservation

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsModifyReservation(
  authorization: string,
  body: CarsmodifyReservationRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`CarsmodifyReservationRequest`](../../doc/models/carsmodify-reservation-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: CarsmodifyReservationRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  configurationId: 4,
  system: 'aft',
  bookingUid: '{{booking_uid}}',
  flightNumber: 'AA1234',
  specialEquipment: [
    'CSI'
  ],
  specialInformation: 'I want a blue car',
  pickupDatetime: '2019-02-25T11:15',
  dropoffDatetime: '2019-02-27T10:30',
  carType: 'ECAR',
};

try {
  const response = await carsApi.mCarsModifyReservation(
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


# Cars Direct Sell Book No Payment

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsDirectSellBookNoPayment(
  authorization: string,
  body: CarsdirectSellBooknoPaymentrequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`CarsdirectSellBooknoPaymentrequest`](../../doc/models/carsdirect-sell-bookno-paymentrequest.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: CarsdirectSellBooknoPaymentrequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  configurationId: 28,
  system: 'aft',
  booktrackId: '{{timestamp}}',
  carType: 'ICAR',
  vendorCode: 'ZL',
  pickupDatetime: '2025-05-19T10:00',
  pickupLocationKey: '_2c_SFxvwYuaw3DxyADA1zvKors6Ppdh4GaEGTBQhDe_Uns6KaFxgwucgExY-h2JR3vxJ4Y6Hbssw0ATKcSgD6MASGDyz24-imM8KwtFKiw7EkC7IpmF5T-SA61v94Jor4DBuhCvCKQb3eyuYnLV1BVDyn6VNTKOtZuUzKqzZr5uKQt-buCMpTypebGwCXbByIrxZ67NMbx1bkD9ij3noljVxQF6RM4eN4tB7kMmeuayv2HJNI5HOtYnLMVePKw7IvKFJsE_zskaGOsbcYYpUiYQk8i8N7y6VmdcPvQrBHVpu8I7OUqrXUQW5-ocxEu_b5kr3SlD7l59TqkV3FFPY0xNs_IMFLzy2suvfRId5NIiaFVwkd6wID07ROns4P5WG38I8LWoZYaYXii6fcffE-Dy_NuVRccV8XfsxoccfipOGEH8E-UZoOIMOq47kI_SF4NqknwObDxEf_V3jugk7NrDrnXb-zK2sLxpLs8__eeaa9fHQ5QQFMncho9gzQGmf90pyoLvf6Nx4I6rz4P1niY4dFThn8Ha-IKlvmVlXJS9_3BDhpmF4x7BYdHItunRqPmRRv54i2CRaYabRGccZF6Uu7Brdcig7XxMd3sg_gOIFIDdD43eMiwOS0boTC_emrsqAB1xW97l25a76HelhtZZljvGNun7w34zvB2L4lRAwKMlW5Wvsu0LXsbGVE8iicmdvkA25rh1RIKRliE43GugQRdyradc25HMtJroKpnHgy40Y_hsHBYoN8nyc6w7da_JkpqKMJSmzlOW1NZ0CYiOiqaj_1Ie_cykAcdYqI12EoIlnMcjk81qG52xyZ9wPMqkAtTmRah1FraFDJdtNDemLkj0keoTUye5lMJIv3gbKwe5w4xb_Yf8KA==',
  dropoffDatetime: '2025-05-20T10:00',
  dropoffLocationKey: '_2c_SFxvwYuaw3DxyADA1zvKors6Ppdh4GaEGTBQhDe_Uns6KaFxgwucgExY-h2JR3vxJ4Y6Hbssw0ATKcSgD6MASGDyz24-imM8KwtFKiw7EkC7IpmF5T-SA61v94Jor4DBuhCvCKQb3eyuYnLV1BVDyn6VNTKOtZuUzKqzZr5uKQt-buCMpTypebGwCXbByIrxZ67NMbx1bkD9ij3noljVxQF6RM4eN4tB7kMmeuayv2HJNI5HOtYnLMVePKw7IvKFJsE_zskaGOsbcYYpUiYQk8i8N7y6VmdcPvQrBHVpu8I7OUqrXUQW5-ocxEu_b5kr3SlD7l59TqkV3FFPY0xNs_IMFLzy2suvfRId5NIiaFVwkd6wID07ROns4P5WG38I8LWoZYaYXii6fcffE-Dy_NuVRccV8XfsxoccfipOGEH8E-UZoOIMOq47kI_SF4NqknwObDxEf_V3jugk7NrDrnXb-zK2sLxpLs8__eeaa9fHQ5QQFMncho9gzQGmf90pyoLvf6Nx4I6rz4P1niY4dFThn8Ha-IKlvmVlXJS9_3BDhpmF4x7BYdHItunRqPmRRv54i2CRaYabRGccZF6Uu7Brdcig7XxMd3sg_gOIFIDdD43eMiwOS0boTC_emrsqAB1xW97l25a76HelhtZZljvGNun7w34zvB2L4lRAwKMlW5Wvsu0LXsbGVE8iicmdvkA25rh1RIKRliE43GugQRdyradc25HMtJroKpnHgy40Y_hsHBYoN8nyc6w7da_JkpqKMJSmzlOW1NZ0CYiOiqaj_1Ie_cykAcdYqI12EoIlnMcjk81qG52xyZ9wPMqkAtTmRah1FraFDJdtNDemLkj0keoTUye5lMJIv3gbKwe5w4xb_Yf8KA==',
  bookerEmail: 'booker@bcdtriptech.com',
  bookerFirstName: 'BookerFirst',
  bookerLastName: 'BookerLast',
  pnrId: 'NQ86M3',
  travelerEmail: 'traveler@bcdtriptech.com',
  travelerFirstName: 'TravelerFirst',
  travelerLastName: 'TravelerLast',
  specialInformation: 'some spec info',
  paymentMethod: 'no_payment',
};

try {
  const response = await carsApi.mCarsDirectSellBookNoPayment(
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


# Cars Cancel Reservation

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsCancelReservation(
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
  bookingUid: '5c867dbbdc8f03103b4daf33',
};

try {
  const response = await carsApi.mCarsCancelReservation(
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


# Cars Get Reservations List

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetReservationsList(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
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

const system = 'aft';

const travelerEmail = 'traveler@bcdtriptech.com';

const status = 'canceled';

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetReservationsList(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
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


# Cars Retrieve Reservations List

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsRetrieveReservationsList(
  authorization: string,
  body: CarsretrieveReservationsListRequest,
  requestOptions?: RequestOptions
): Promise<ApiResponse<void>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `authorization` | `string` | Header, Required | - |
| `body` | [`CarsretrieveReservationsListRequest`](../../doc/models/carsretrieve-reservations-list-request.md) | Body, Required | - |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

This method returns an [`ApiResponse`](../../doc/api-response.md) instance.

## Example Usage

```ts
const authorization = 'Signature {{signature}}';

const body: CarsretrieveReservationsListRequest = {
  apiKey: '{{ASB_API_KEY}}',
  timestamp: '{{timestamp}}',
  nonce: '{{nonce}}',
  locale: 'en_US',
  customerIp: '127.0.0.1',
  sessionId: '{{session_id}}',
  userAgent: 'curl/7.64.0',
  system: 'aft',
  travelerEmail: 'traveler@bcdtriptech.com',
  limit: 20,
  offset: 0,
  filters: {  },
};

try {
  const response = await carsApi.mCarsRetrieveReservationsList(
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


# Cars Get Reservation Details

:information_source: **Note** This endpoint does not require authentication.

```ts
async mCarsGetReservationDetails(
  apiKey: string,
  timestamp: string,
  nonce: string,
  locale: string,
  customerIp: string,
  sessionId: string,
  userAgent: string,
  system: string,
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

const bookingUid = '5c867dbbdc8f03103b4daf33';

const authorization = 'Signature {{signature}}';

try {
  const response = await carsApi.mCarsGetReservationDetails(
    apiKey,
    timestamp,
    nonce,
    locale,
    customerIp,
    sessionId,
    userAgent,
    system,
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

