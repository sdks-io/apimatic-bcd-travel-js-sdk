
# Airget Checkout Data Request

*This model accepts additional fields of type unknown.*

## Structure

`AirgetCheckoutDataRequest`

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
| `system` | `string` | Required | - |
| `configurationId` | `number` | Required | - |
| `fareGroupKey` | `string` | Required | - |
| `tspmTravelerId` | `string` | Required | - |
| `tspmCompanyId` | `string` | Required | - |
| `additionalProperties` | `Record<string, unknown>` | Optional | - |

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
  "system": "aft",
  "configuration_id": 4,
  "fare_group_key": "UGRKFI0kToRXdO6LZZ-nyiYlCrO-R5i98sOkLeQPnMZJjqtd3Kc5Pu7RORES1fIqWGc3sx2eSHF1ZuVEutmnxkdVTZ83X_S2_dKoB_u5iyjaPqT0VfPy6rkrteSd2xIInKK_NrQvmktn4n_oPNJDbh9Mpo3BY487UuAtNZcn_S9JHdbkmjtXhbdLUMhcsvScOys8xK-O5ce-1_DcddScO-fytwjfJY-EbxXCEY1CTRozZ0Mbl6EvbB6J3SMH4rtlSE0pmJxRBW4DUOXjoFWqM1fMD7AFkihDRsXWFz65Rz6yQedcKiYR8yJ0MDiT34JpPLPb25Lb3fwHDeWlgzdg2S0kKW219yxDGY3wkYG1fWRXvWTkcXoUHJEgV7kJBMOJCOK295KF1TDUdJrBcvVD_amDVjg5aDOEUsKMqoUOBAm0dOG046lzUPYZh9dl8P1HsbjdMF-b3GZhulY0igBjzOaVvF4L7iBgpZLAy_s6UEjCIpQTaGrPFBWUP_nGxj9eybCMRxCDoxtW_JJxCLvJVDwucd849O8Uv5FaRmY-4-be8w5dK5grDpt1kB6FN-3_nYQ7mVxz48bdyz52iT09cA==",
  "tspm_traveler_id": "24.9999999999995",
  "tspm_company_id": "20.999999999999",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

