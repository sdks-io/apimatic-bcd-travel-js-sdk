
# Ping Getresponse

*This model accepts additional fields of type unknown.*

## Structure

`PingGetresponse`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `ping` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "ping": "pong, v2.0",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

