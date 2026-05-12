
# Basic Authentication



Documentation for accessing and setting credentials for basic.

## Auth Credentials

| Name | Type | Description | Setter |
|  --- | --- | --- | --- |
| username | `string` | The username to use with basic authentication | `username` |
| password | `string` | The password to use with basic authentication | `password` |



**Note:** Auth credentials can be set using `basicCredentials` object in the client.

## Usage Example

### Client Initialization

You must provide credentials in the client as shown in the following code snippet.

```ts
import { Client } from 'apimatic-bcd-travel-sdk';

const client = new Client({
  basicCredentials: {
    username: 'Username',
    password: 'Password'
  },
});
```


