### Description
Esta API permite obtener los Rates de ShipStation

**HTTP Method:** `Post`

**Endpoint:** `api/v1.0/webhooks?appSource=erp&customerId={customerId}&parms={parms}&secretKey={secretKey}`
#### Example:
```
api/v1.0/webhooks?appSource=erp&customerId=cus_OTWT9NtE1HGhmP&parms=WTNWelgwOVVWMVE1VG5SRk1VaEhhRzFRc2tfTkRNMlpHVXpObVV0TTJSaVpTMDBOekJtTFRsbE5UUXRNemsxTVdZMk16WXdZV1Zp&secretKey=sk_NDM2ZGUzNmUtM2RiZS00NzBmLTllNTQtMzk1MWY2MzYwYWVi
``` 

**Request:** 

```
{
    "CustomerId": "cus_Ohex6sITWij0ja",
    "EnvironmentId": "env_48098549e77f418b974a80455600944a",
    "CompanyId": "FBFFF439-569B-ED11-BFF5-000D3A71DACD",
    "ProcessMethod": "GetRates",
    "JsonRequest": "{\"carrierCode\":\"fedex\",\"serviceCode\":null,\"packageCode\":null,\"fromPostalCode\":\"78703\",\"toState\":\"DC\",\"toCountry\":\"US\",\"toPostalCode\":\"20500\",\"toCity\":\"Washington\",\"weight\":{\"value\":3,\"units\":\"ounces\"},\"dimensions\":{\"units\":\"inches\",\"length\":7,\"width\":5,\"height\":6},\"confirmation\":\"delivery\",\"residential\":false}"
}
```

**Response:** 

```
{
    "customerId": "cus_Ohex6sITWij0ja",
    "environmentId": "env_48098549e77f418b974a80455600944a",
    "processMethod": "GetRates",
    "userId": null,
    "result":"[{\"ServiceName\":\"FedEx First Overnight\®\",\"ServiceCode\":\"fedex_first_overnight\",\"ShipmentCost\":124.18,\"OtherCost\":20.80},{\"ServiceName\":\"FedEx Priority Overnight\®\",\"ServiceCode\":\"fedex_priority_overnight\",\"ShipmentCost\":40.07,\"OtherCost\":6.71},{\"ServiceName\":\"FedEx Standard Overnight\®\",\"ServiceCode\":\"fedex_standard_overnight\",\"ShipmentCost\":39.27,\"OtherCost\":6.58},{\"ServiceName\":\"FedEx 2Day\® A.M.\",\"ServiceCode\":\"fedex_2day_am\",\"ShipmentCost\":24.29,\"OtherCost\":4.07},{\"ServiceName\":\"FedEx 2Day\®\",\"ServiceCode\":\"fedex_2day\",\"ShipmentCost\":18.38,\"OtherCost\":3.08},{\"ServiceName\":\"FedEx Express Saver\®\",\"ServiceCode\":\"fedex_express_saver\",\"ShipmentCost\":17.17,\"OtherCost\":2.88},{\"ServiceName\":\"FedEx Ground\®\",\"ServiceCode\":\"fedex_ground\",\"ShipmentCost\":10.2,\"OtherCost\":1.58},{\"ServiceName\":\"FedEx Home Delivery\®\",\"ServiceCode\":\"fedex_home_delivery\",\"ShipmentCost\":10.2,\"OtherCost\":4.78}]",
    "error": ""
}
```

**Curl**
```
curl --location 'https://localhost:5001/api/v1.0/webhooks?appSource=erp&customerId=cus_Ohex6sITWij0ja&parms=WTNWelgwOW9aWGcyYzBsVVYybHFNR3Boc2tfT0dNeU1HUXlZelF0WWpaaVppMDBaalZoTFdGbE1XRXRNR1JpTVdOaU1XWTVaR0k1&secretKey=sk_OGMyMGQyYzQtYjZiZi00ZjVhLWFlMWEtMGRiMWNiMWY5ZGI5' \
--header 'Content-Type: application/json' \
--data '{
    "CustomerId": "cus_Ohex6sITWij0ja",
    "EnvironmentId": "env_48098549e77f418b974a80455600944a",
    "CompanyId": "{FBFFF439-569B-ED11-BFF5-000D3A71DACD}",
    "ProcessMethod": "GetRates",
    "JsonRequest": "{\"carrierCode\":\"fedex\",\"serviceCode\":null,\"packageCode\":null,\"fromPostalCode\":\"78703\",\"toState\":\"DC\",\"toCountry\":\"US\",\"toPostalCode\":\"20500\",\"toCity\":\"Washington\",\"weight\":{\"value\":3,\"units\":\"ounces\"},\"dimensions\":{\"units\":\"inches\",\"length\":7,\"width\":5,\"height\":6},\"confirmation\":\"delivery\",\"residential\":false}"
}'
```