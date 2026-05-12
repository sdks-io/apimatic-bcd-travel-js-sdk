
# Getting Started with ASB API

## Install the Package

Run the following command from your project directory to install the package from npm:

```bash
npm install apimatic-bcd-travel-sdk@0.0.2
```

For additional package details, see the [Npm page for the apimatic-bcd-travel-sdk@0.0.2 npm](https://www.npmjs.com/package/apimatic-bcd-travel-sdk/v/0.0.2).

## Test the SDK

To validate the functionality of this SDK, you can execute all tests located in the `test` directory. This SDK utilizes `Jest` as both the testing framework and test runner.

To run the tests, navigate to the root directory of the SDK and execute the following command:

```bash
npm run test
```

Or you can also run tests with coverage report:

```bash
npm run test:coverage
```

## Initialize the API Client

**_Note:_** Documentation for the client can be found [here.](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/client.md)

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| version | `string` | *Default*: `'DefaultParameterValue'` |
| environment | [`Environment`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/README.md#environments) | The API environment. <br> **Default: `Environment.Production`** |
| timeout | `number` | Timeout for API calls.<br>*Default*: `0` |
| httpClientOptions | [`Partial<HttpClientOptions>`](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/http-client-options.md) | Stable configurable http client options. |
| unstableHttpClientOptions | `any` | Unstable configurable http client options. |

The API client can be initialized as follows:

### Code-Based Client Initialization

```ts
import { Client, Environment } from 'apimatic-bcd-travel-sdk';

const client = new Client({
  timeout: 0,
  environment: Environment.Production,
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

See the [Configuration-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/configuration-based-client-initialization.md) section for details.

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

See the [Environment-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/environment-based-client-initialization.md) section for details.

## Environments

The SDK can be configured to use a different environment for making API calls. Available environments are:

### Fields

| Name | Description |
|  --- | --- |
| Production | **Default** |
| Environment2 | - |

## List of APIs

* [Hotels](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/hotels.md)
* [Cars](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/cars.md)
* [Air-Fare-Search-Simple](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/air-fare-search-simple.md)
* [Air-Fare-Search-Select-Seat](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/air-fare-search-select-seat.md)
* [Air-Fare-Search-Optional-Services](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/air-fare-search-optional-services.md)
* [Air-Availability-Return-Flight](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/air-availability-return-flight.md)
* [Air](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/air.md)
* [V2 1](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/v2-1.md)
* [V2 0](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/controllers/v2-0.md)

## SDK Infrastructure

### Configuration

* [HttpClientOptions](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/http-client-options.md)
* [RetryConfiguration](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/retry-configuration.md)
* [ProxySettings](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/proxy-settings.md)
* [Configuration-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/configuration-based-client-initialization.md)
* [Environment-Based Client Initialization](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/environment-based-client-initialization.md)

### HTTP

* [HttpRequest](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/http-request.md)

### Utilities

* [ApiResponse](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/api-response.md)
* [ApiError](https://www.github.com/sdks-io/apimatic-bcd-travel-js-sdk/tree/0.0.2/doc/api-error.md)

