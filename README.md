
# Getting Started with BCD Travel API

## Introduction

The Travel Expenses API allows clients and partners to view transaction data (a.k.a. “expense data”) in real-time. This API allows integration with your application to view your corporate travel expenses.

Modify provided Postman environment `Travel Expenses API OAuth 2.0` with your `ClientId`, `ClientSecret`, and environment URLs (`AuthAPI` and `ExpensesAPI`). The `AuthToken` should auto populate by pre-request script associated with the collection or you can use `Generate OAuth 2.0 Token` request.

## Install the Package

Run the following command from your project directory to install the package from npm:

```bash
npm install apimatic-bcd-travel-sdk@0.0.1
```

For additional package details, see the [Npm page for the apimatic-bcd-travel-sdk@0.0.1 npm](https://www.npmjs.com/package/apimatic-bcd-travel-sdk/v/0.0.1).

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| version | `string` | *Default*: `'DefaultParameterValue'` |
| environment | [`Environment`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/README.md#environments) | The API environment. <br> **Default: `Environment.Production`** |
| timeout | `number` | Timeout for API calls.<br>*Default*: `30000` |
| httpClientOptions | [`Partial<HttpClientOptions>`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/http-client-options.md) | Stable configurable http client options. |
| unstableHttpClientOptions | `any` | Unstable configurable http client options. |
| logging | [`PartialLoggingOptions`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/partial-logging-options.md) | Logging Configuration to enable logging |
| bearerCredentials | [`BearerCredentials`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/auth/oauth-2-bearer-token.md) | The credential object for bearer |
| basicCredentials | [`BasicCredentials`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/auth/basic-authentication.md) | The credential object for basic |

The API client can be initialized as follows:

### Code-Based Client Initialization

```ts
import { Client, Environment, LogLevel } from 'apimatic-bcd-travel-sdk';

const client = new Client({
  bearerCredentials: {
    accessToken: 'AccessToken'
  },
  basicCredentials: {
    username: 'Username',
    password: 'Password'
  },
  timeout: 30000,
  environment: Environment.Production,
  logging: {
    logLevel: LogLevel.Info,
    logRequest: {
      logBody: true
    },
    logResponse: {
      logHeaders: true
    }
  },
  version: 'DefaultParameterValue',
});
```

### Configuration-Based Client Initialization

```ts
import * as path from 'path';
import * as fs from 'fs';
import { Client } from 'apimatic-bcd-travel-sdk';

// Provide absolute path for the configuration file
const absolutePath = path.resolve('./config.json');

// Read the configuration file content
const fileContent = fs.readFileSync(absolutePath, 'utf-8');

// Initialize client from JSON configuration content
const client = Client.fromJsonConfig(fileContent);
```

See the [Configuration-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/configuration-based-client-initialization.md) section for details.

### Environment-Based Client Initialization

```ts
import * as dotenv from 'dotenv';
import * as path from 'path';
import * as fs from 'fs';
import { Client } from 'apimatic-bcd-travel-sdk';

// Optional - Provide absolute path for the .env file
const absolutePath = path.resolve('./.env');

if (fs.existsSync(absolutePath)) {
  // Load environment variables from .env file
  dotenv.config({ path: absolutePath, override: true });
}

// Initialize client using environment variables
const client = Client.fromEnvironment(process.env);
```

See the [Environment-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/environment-based-client-initialization.md) section for details.

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| Production | **Default** |
| Environment2 | - |

## Authorization

This API uses the following authentication schemes.

* [`bearer (OAuth 2 Bearer token)`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/auth/oauth-2-bearer-token.md)
* [`basic (Basic Authentication)`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/auth/basic-authentication.md)

## List of APIs

* [Search Expenses](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/search-expenses.md)
* [Retrieveversions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/retrieveversions.md)
* [Hotels](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/hotels.md)
* [Cars](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/cars.md)
* [Air-Fare-Search-Simple](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/air-fare-search-simple.md)
* [Air-Fare-Search-Select-Seat](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/air-fare-search-select-seat.md)
* [Air-Fare-Search-Optional-Services](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/air-fare-search-optional-services.md)
* [Air-Availability-Return-Flight](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/air-availability-return-flight.md)
* [Air](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/air.md)
* [V2 1](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/v2-1.md)
* [V2 0](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/controllers/v2-0.md)

## SDK Infrastructure

### Configuration

* [HttpClientOptions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/http-client-options.md)
* [RetryConfiguration](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/retry-configuration.md)
* [ProxySettings](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/proxy-settings.md)
* [Configuration-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/configuration-based-client-initialization.md)
* [Environment-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/environment-based-client-initialization.md)
* [PartialLoggingOptions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/partial-logging-options.md)
* [PartialRequestLoggingOptions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/partial-request-logging-options.md)
* [PartialResponseLoggingOptions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/partial-response-logging-options.md)
* [LoggerInterface](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/logger-interface.md)

### HTTP

* [HttpRequest](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/api-response.md)
* [ApiError](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.1/doc/api-error.md)

