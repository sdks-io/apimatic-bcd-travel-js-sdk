
# Options

*This model accepts additional fields of type unknown.*

## Structure

`Options`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `requestQuoteId` | `boolean` | Required | - |
| `segmentsOnly` | `boolean` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "request_quote_id": false,
  "segments_only": false,
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

