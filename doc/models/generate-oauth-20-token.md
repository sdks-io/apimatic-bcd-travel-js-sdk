
# Generate Oauth 20 Token

*This model accepts additional fields of type unknown.*

## Structure

`GenerateOauth20Token`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `accessToken` | `string` | Required | - |
| `expiresIn` | `number` | Required | - |
| `tokenType` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "access_token": "Token",
  "expires_in": 3600,
  "token_type": "Bearer",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

