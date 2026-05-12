
# Get Configurations POST Request

## Structure

`GetConfigurationsPOSTRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `apiKey` | `string` | Required | - |
| `timestamp` | `string` | Required | - |
| `nonce` | `string` | Required | - |
| `locale` | `string` | Required | - |
| `customerIp` | `string` | Required | - |
| `sessionId` | `string` | Required | - |
| `userAgent` | `string` | Required | - |
| `entityId` | `number` | Required | - |
| `system` | `string` | Required | - |
| `tspmCompanyId` | `string` | Required | - |
| `tspmTravelerId` | `string` | Required | - |
| `clientReportableData` | [`ClientReportableDatum[]`](../../doc/models/client-reportable-datum.md) | Required | - |
| `pnrId` | `string` | Required | - |

## Example (as JSON)

```json
{
  "api_key": "{{ASB_API_KEY}}",
  "timestamp": "{{timestamp}}",
  "nonce": "{{nonce}}",
  "locale": "en_US",
  "customer_ip": "127.0.0.1",
  "session_id": "{{session_id}}",
  "user_agent": "curl/7.64.0",
  "entity_id": 4,
  "system": "aft",
  "tspm_company_id": "20.14881",
  "tspm_traveler_id": "24.100000037",
  "client_reportable_data": [
    {
      "code": "AFT.COMMON.CRD.vip_person",
      "answer": "ans1"
    }
  ],
  "pnr_id": "NQ86M3"
}
```

