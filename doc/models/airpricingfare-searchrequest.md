
# Airpricingfare Searchrequest

*This model accepts additional fields of type unknown.*

## Structure

`AirpricingfareSearchrequest`

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
| `currency` | `string` | Required | - |
| `fareGroupKey` | `string` | Required | - |
| `flightOptionKeys` | `string[]` | Required | - |
| `optionalServiceKeys` | `string[]` | Required | - |
| `fareFamilies` | `boolean` | Required | - |
| `travelers` | [`Traveler[]`](../../doc/models/traveler.md) | Required | - |
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
  "currency": "UAH",
  "fare_group_key": "UGRKFI0kToRXdO6LZZ-nyiYlCrO-R5i98sOkLeQPnMZJjqtd3Kc5Pu7RORES1fIqWGc3sx2eSHF1ZuVEutmnxkdVTZ83X_S2_dKoB_u5iyjaPqT0VfPy6rkrteSd2xIInKK_NrQvmktn4n_oPNJDbh9Mpo3BY487UuAtNZcn_S9JHdbkmjtXhbdLUMhcsvScOys8xK-O5ce-1_DcddScO-fytwjfJY-EbxXCEY1CTRozZ0Mbl6EvbB6J3SMH4rtlSE0pmJxRBW4DUOXjoFWqM1fMD7AFkihDRsXWFz65Rz6yQedcKiYR8yJ0MDiT34JpPLPb25Lb3fwHDeWlgzdg2S0kKW219yxDGY3wkYG1fWRXvWTkcXoUHJEgV7kJBMOJCOK295KF1TDUdJrBcvVD_amDVjg5aDOEUsKMqoUOBAm0dOG046lzUPYZh9dl8P1HsbjdMF-b3GZhulY0igBjzOaVvF4L7iBgpZLAy_s6UEjCIpQTaGrPFBWUP_nGxj9eybCMRxCDoxtW_JJxCLvJVDwucd849O8Uv5FaRmY-4-be8w5dK5grDpt1kB6FN-3_nYQ7mVxz48bdyz52iT09cA==",
  "flight_option_keys": [
    "HM5hS4x_2__K_ivF6ZlLg3poDWcXq0DHYhNIf4g7PvlirSjWHqJvBkyH54fLR6-rNGwCJ5kCd0bTdwW-iXehwdNL-cswK2GK6TQZ_l3_MC596E2f6N13reUl6H3lnLKaArl6wqeo1TLaPY2NC4asykl0vxrkTnvm4N0exyw0FHw__TiZSDE7bGzaMajXsfuzPDRTbXmvoD59W-R8nYjesShznx090_muKrSZrEJ9JQiWW5Hzn9prSWxqDZ9OxsWW8Vv-VMx1nCsoykvA3aM4hl3Q4XqUYryWfhHuvEVJ6G1szhnsNdj7bsJLGBTmCVwUZsFaUsKBoRa2TgPQtRPHeD9-f9FxEH5X5m5LvKCjboDn81VeD-jbqKCx6pBmjiPwBmsKSIu1k5lLTvdGhNsEgNJCsMICX7Vlz3697A58AWOpKzGlJIGWwNS8KMXB5h4DwWf70XcPfXZkQzUk9MMDwAzh0n6Z_tRzvmiekJgXp-waRrKLgws9ITmwF1QHsPjnWDlZwmCLC4T1iKcthsFAjuK7BKKbzmbLJ7mUla7SBfMhrrETkXPLby0W_udTl0Pd-5owgPmb4OpryIMoVepxCWJ643LmKw==",
    "4q1pMpVsdeJ0BLTqvso_hSd7d3VIaZyQCHZMgO-UMSgfzU8QvavhmUU2PpL7Mb0qPKs7nlVaBYrqBx_KrgREuLMichqkVdNp3MPwUVr8Pubn8FSeY9fpIdlwNbiz9659Uxd6AHm8T1_AQZT7j5h3MNOZ7RhHIR7jxdoOixDHwv2yB2qLaDZmVzftB_N28qFLf6_U_sAEOvq1psC1l0e-4Wzh69U6FT1PmELIN5bovOKNTqI8iqoumZafdk2Dc_PMYTQJAlMRi61o1-zRo2RFMBYWtVmPcDqPnFaJbG7xnGj9MOCVPCrFhNv9xN_GuXWviTweiC2wAno5NJARlw8vaJRf7mhTkiIaOEsXafnssWMOqsZIYfSBlmOyCNXinf5viRcRs9G_-26t1f2Z7zQkmaCehue7bdAjuVuGf-smuqOallUm5ewIA_fRzbIOdrtdbBL7uZGXb5_pk97LVYpnK4iYESBln9obnrzDoYdNWLnOSV-V7jVOBh-_xFzyj5K8AswtTPEYJxyncwnA1Y40Cc7oQ1PljX0olhR4lftQ7GuwOm8qstr2H9bHKtIEk7rSy5Lkgx59DWsHmkQ6T2-u-DpkihUaOw=="
  ],
  "optional_service_keys": [
    "k834yMQC7f-eolNOkqJTRa9TY3ViYSBFcXVpcG1lbnSSojMysVVwIHRvIDcwIGxiLzMyIGtnkqJCR6dCYWdnYWdlkqJTULJTcG9ydGluZyBFcXVpcG1lbnS-U0NVQkEgRVFVSVBNRU5UIFVQIFRPNzBMQiAzMktHkgABokVBoUO2MzU0dGFUaXRIeHRHa1VSS3RadjBJQ5GhMaMwSDCRoTGhMg=="
  ],
  "fare_families": false,
  "travelers": [
    {
      "traveler_type": "adult",
      "ff_numbers": [
        {
          "airline_code": "KL",
          "ff_number": "222111",
          "exampleAdditionalProperty": {
            "key1": "val1",
            "key2": "val2"
          }
        }
      ],
      "exampleAdditionalProperty": {
        "key1": "val1",
        "key2": "val2"
      }
    }
  ],
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

