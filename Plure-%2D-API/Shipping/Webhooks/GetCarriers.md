### Description
Esta API permite obtener los Carriers configurados en ShipStation

**HTTP Method:** `Post`

**Endpoint:** `api/v1.0/webhooks?appSource=erp&customerId={customerId}&parms={parms}&secretKey={secretKey}`
#### Example:
```
api/v1.0/webhooks?appSource=erp&customerId=cus_OTWT9NtE1HGhmP&parms=WTNWelgwOVVWMVE1VG5SRk1VaEhhRzFRc2tfTkRNMlpHVXpObVV0TTJSaVpTMDBOekJtTFRsbE5UUXRNemsxTVdZMk16WXdZV1Zp&secretKey=sk_NDM2ZGUzNmUtM2RiZS00NzBmLTllNTQtMzk1MWY2MzYwYWVi
``` 

**Request:** 

```
{
    "ProcessMethod": "GetCarriers"
}
```

**Response:** 

```
{
    "customerId": "cus_OTWT9NtE1HGhmP",
    "environmentId": null,
    "processMethod": "GetCarriers",
    "userId": null,
    "result":"[{\"Name\":\"Stamps.com\",\"Code\":\"stamps_com\",\"AccountNumber\":null,\"RequiresFundedAccount\":true,\"Balance\":0.0,\"Nickname\":\"Free\",\"ShippingProviderId\":262752,\"Primary\":true,\"Services\":[{\"Code\":\"usps_priority_mail\",\"Name\":\"USPS Priority Mail\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_priority_mail_express\",\"Name\":\"USPS Priority Mail Express\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_parcel_select\",\"Name\":\"USPS Parcel Select Ground\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_first_class_mail\",\"Name\":\"USPS First Class Mail\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_media_mail\",\"Name\":\"USPS Media Mail\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_ground_advantage\",\"Name\":\"USPS Ground Advantage\",\"Domestic\":true,\"International\":false},{\"Code\":\"usps_priority_mail_international\",\"Name\":\"USPS Priority Mail Intl\",\"Domestic\":false,\"International\":true},{\"Code\":\"usps_priority_mail_express_international\",\"Name\":\"USPS Priority Mail Express Intl\",\"Domestic\":false,\"International\":true},{\"Code\":\"usps_first_class_mail_international\",\"Name\":\"USPS First Class Mail Intl\",\"Domestic\":false,\"International\":true},{\"Code\":\"globalpost_parcel_select_smart_saver\",\"Name\":\"GlobalPost Parcel Select SmartSaver\",\"Domestic\":true,\"International\":false}]},{\"Name\":\"UPS by ShipStation\",\"Code\":\"ups_walleted\",\"AccountNumber\":null,\"RequiresFundedAccount\":true,\"Balance\":0.0,\"Nickname\":null,\"ShippingProviderId\":262753,\"Primary\":true,\"Services\":[{\"Code\":\"ups_ground_saver\",\"Name\":\"UPS\® Ground Saver\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_ground\",\"Name\":\"UPS\® Ground\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_ground_international\",\"Name\":\"UPS Ground\® (International)\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_standard_international\",\"Name\":\"UPS Standard\®\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_3_day_select\",\"Name\":\"UPS 3 Day Select\®\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_worldwide_saver\",\"Name\":\"UPS Worldwide Saver\®\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_worldwide_express\",\"Name\":\"UPS Worldwide Express\®\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_2nd_day_air\",\"Name\":\"UPS 2nd Day Air\®\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_worldwide_expedited\",\"Name\":\"UPS Worldwide Expedited\®\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_worldwide_express_plus\",\"Name\":\"UPS Worldwide Express Plus\®\",\"Domestic\":false,\"International\":true},{\"Code\":\"ups_2nd_day_air_am\",\"Name\":\"UPS 2nd Day Air AM\®\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_next_day_air_saver\",\"Name\":\"UPS Next Day Air Saver\®\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_next_day_air\",\"Name\":\"UPS Next Day Air\®\",\"Domestic\":true,\"International\":false},{\"Code\":\"ups_next_day_air_early_am\",\"Name\":\"UPS Next Day Air\® Early\",\"Domestic\":true,\"International\":false}]}]",
    "error": ""
}
```