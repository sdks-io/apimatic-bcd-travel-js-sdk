
# Segment Option

*This model accepts additional fields of type unknown.*

## Structure

`SegmentOption`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `segmentIdRef` | `number` | Required | - |
| `classOfService` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

## Example (as JSON)

```json
{
  "segment_id_ref": 1,
  "class_of_service": "Y",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

