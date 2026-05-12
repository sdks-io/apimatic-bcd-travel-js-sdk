
# Carsdirect Sell Bookno Paymentrequest

*This model accepts additional fields of type unknown.*

## Structure

`CarsdirectSellBooknoPaymentrequest`

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
| `configurationId` | `number` | Required | - |
| `system` | `string` | Required | - |
| `booktrackId` | `string` | Required | - |
| `carType` | `string` | Required | - |
| `vendorCode` | `string` | Required | - |
| `pickupDatetime` | `string` | Required | - |
| `pickupLocationKey` | `string` | Required | - |
| `dropoffDatetime` | `string` | Required | - |
| `dropoffLocationKey` | `string` | Required | - |
| `bookerEmail` | `string` | Required | - |
| `bookerFirstName` | `string` | Required | - |
| `bookerLastName` | `string` | Required | - |
| `pnrId` | `string` | Required | - |
| `travelerEmail` | `string` | Required | - |
| `travelerFirstName` | `string` | Required | - |
| `travelerLastName` | `string` | Required | - |
| `specialInformation` | `string` | Required | - |
| `paymentMethod` | `string` | Required | - |
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
  "configuration_id": 28,
  "system": "aft",
  "booktrack_id": "{{timestamp}}",
  "car_type": "ICAR",
  "vendor_code": "ZL",
  "pickup_datetime": "2025-05-19T10:00",
  "pickup_location_key": "_2c_SFxvwYuaw3DxyADA1zvKors6Ppdh4GaEGTBQhDe_Uns6KaFxgwucgExY-h2JR3vxJ4Y6Hbssw0ATKcSgD6MASGDyz24-imM8KwtFKiw7EkC7IpmF5T-SA61v94Jor4DBuhCvCKQb3eyuYnLV1BVDyn6VNTKOtZuUzKqzZr5uKQt-buCMpTypebGwCXbByIrxZ67NMbx1bkD9ij3noljVxQF6RM4eN4tB7kMmeuayv2HJNI5HOtYnLMVePKw7IvKFJsE_zskaGOsbcYYpUiYQk8i8N7y6VmdcPvQrBHVpu8I7OUqrXUQW5-ocxEu_b5kr3SlD7l59TqkV3FFPY0xNs_IMFLzy2suvfRId5NIiaFVwkd6wID07ROns4P5WG38I8LWoZYaYXii6fcffE-Dy_NuVRccV8XfsxoccfipOGEH8E-UZoOIMOq47kI_SF4NqknwObDxEf_V3jugk7NrDrnXb-zK2sLxpLs8__eeaa9fHQ5QQFMncho9gzQGmf90pyoLvf6Nx4I6rz4P1niY4dFThn8Ha-IKlvmVlXJS9_3BDhpmF4x7BYdHItunRqPmRRv54i2CRaYabRGccZF6Uu7Brdcig7XxMd3sg_gOIFIDdD43eMiwOS0boTC_emrsqAB1xW97l25a76HelhtZZljvGNun7w34zvB2L4lRAwKMlW5Wvsu0LXsbGVE8iicmdvkA25rh1RIKRliE43GugQRdyradc25HMtJroKpnHgy40Y_hsHBYoN8nyc6w7da_JkpqKMJSmzlOW1NZ0CYiOiqaj_1Ie_cykAcdYqI12EoIlnMcjk81qG52xyZ9wPMqkAtTmRah1FraFDJdtNDemLkj0keoTUye5lMJIv3gbKwe5w4xb_Yf8KA==",
  "dropoff_datetime": "2025-05-20T10:00",
  "dropoff_location_key": "_2c_SFxvwYuaw3DxyADA1zvKors6Ppdh4GaEGTBQhDe_Uns6KaFxgwucgExY-h2JR3vxJ4Y6Hbssw0ATKcSgD6MASGDyz24-imM8KwtFKiw7EkC7IpmF5T-SA61v94Jor4DBuhCvCKQb3eyuYnLV1BVDyn6VNTKOtZuUzKqzZr5uKQt-buCMpTypebGwCXbByIrxZ67NMbx1bkD9ij3noljVxQF6RM4eN4tB7kMmeuayv2HJNI5HOtYnLMVePKw7IvKFJsE_zskaGOsbcYYpUiYQk8i8N7y6VmdcPvQrBHVpu8I7OUqrXUQW5-ocxEu_b5kr3SlD7l59TqkV3FFPY0xNs_IMFLzy2suvfRId5NIiaFVwkd6wID07ROns4P5WG38I8LWoZYaYXii6fcffE-Dy_NuVRccV8XfsxoccfipOGEH8E-UZoOIMOq47kI_SF4NqknwObDxEf_V3jugk7NrDrnXb-zK2sLxpLs8__eeaa9fHQ5QQFMncho9gzQGmf90pyoLvf6Nx4I6rz4P1niY4dFThn8Ha-IKlvmVlXJS9_3BDhpmF4x7BYdHItunRqPmRRv54i2CRaYabRGccZF6Uu7Brdcig7XxMd3sg_gOIFIDdD43eMiwOS0boTC_emrsqAB1xW97l25a76HelhtZZljvGNun7w34zvB2L4lRAwKMlW5Wvsu0LXsbGVE8iicmdvkA25rh1RIKRliE43GugQRdyradc25HMtJroKpnHgy40Y_hsHBYoN8nyc6w7da_JkpqKMJSmzlOW1NZ0CYiOiqaj_1Ie_cykAcdYqI12EoIlnMcjk81qG52xyZ9wPMqkAtTmRah1FraFDJdtNDemLkj0keoTUye5lMJIv3gbKwe5w4xb_Yf8KA==",
  "booker_email": "booker@bcdtriptech.com",
  "booker_first_name": "BookerFirst",
  "booker_last_name": "BookerLast",
  "pnr_id": "NQ86M3",
  "traveler_email": "traveler@bcdtriptech.com",
  "traveler_first_name": "TravelerFirst",
  "traveler_last_name": "TravelerLast",
  "special_information": "some spec info",
  "payment_method": "no_payment",
  "exampleAdditionalProperty": {
    "key1": "val1",
    "key2": "val2"
  }
}
```

