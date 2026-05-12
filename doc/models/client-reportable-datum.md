
# Client Reportable Datum

*This model accepts additional fields of type unknown.*

## Structure

`ClientReportableDatum`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `code` | `string` | Required | - |
| `answer` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "code": "AFT.COMMON.CRD.vip_person",
  "answer": "ans1",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

