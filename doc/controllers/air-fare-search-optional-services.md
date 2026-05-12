# Air-Fare-Search-Optional-Services

```ts
const airFareSearchOptionalServicesApi = new AirFareSearchOptionalServicesApi(client);
```

## Class Name

`AirFareSearchOptionalServicesApi`


# Air Get Checkout Data

:information_source: **Note** This endpoint does not require authentication.

```ts
async mAirGetCheckoutData(
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

const body = '{\n	"api_key": "{{ASB_API_KEY}}",\n	"timestamp": "{{timestamp}}",\n	"nonce": "{{nonce}}",\n	"locale": "en_US",\n	"customer_ip": "127.0.0.1",\n	"session_id": "{{session_id}}",\n	"user_agent": "curl/7.64.0",\n	"system": "aft",\n	\n	"configuration_id": {{configuration_id}},\n    "fare_group_key": "{{fare_group_key}}",\n    "tspm_traveler_id": "{{tspm_traveler_id}}",\n    "tspm_company_id": "{{tspm_company_id}}"\n}';

try {
  const response = await airFareSearchOptionalServicesApi.mAirGetCheckoutData(
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

