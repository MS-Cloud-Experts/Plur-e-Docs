### Description
Esta API permite crear una o muchas ordernes en ShipStation

**HTTP Method:** `Post`

**Endpoint:** `api/v1.0/webhooks?appSource=erp&customerId={customerId}&parms={parms}&secretKey={secretKey}`
#### Example:
```
api/v1.0/webhooks?appSource=erp&customerId=cus_OTWT9NtE1HGhmP&parms=WTNWelgwOVVWMVE1VG5SRk1VaEhhRzFRc2tfTkRNMlpHVXpObVV0TTJSaVpTMDBOekJtTFRsbE5UUXRNemsxTVdZMk16WXdZV1Zp&secretKey=sk_NDM2ZGUzNmUtM2RiZS00NzBmLTllNTQtMzk1MWY2MzYwYWVi
``` 

**Request:** 

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "CreateOrUpdatePackageShipment",
    "companyId": "bc79d441-b4a4-ee11-be36-7c1e520783d3",
    "jsonRequest": "[{\"ShippingAgentCode\":\"ups\",\"ShippingAgentService\":\"ups_ground\",\"PackageNo\":1,\"OrderId\":0,\"OrderKey\":\"\",\"SourceNo\":\"WHSESHIP-000222\",\"PackingDate\":\"2024-02-27T20:36:02.6100000Z\",\"CustomerUsername\":\"3rdAVEKITEREPAIR\",\"CustomerEmail\":\"diego.rozo@mscloudexperts.com\",\"BillTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSAPlur-eV3\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"},\"ShipTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSAPlur-eV3\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"},\"Lines\":[{\"PackageNo\":1,\"ItemNo\":\"K3KOSWTCH\",\"Name\":\"K3KOSWTCH\",\"QtyToHandle\":1,\"LineNo\":1000,\"SourceNo\":\"SOB2B-301734\",\"WarehouseDocumentNo\":\"WHSEPICK-00036\",\"WarehouseLineNo\":10000,\"VariantCode\":\"012011\",\"ItemPrice\":1469}],\"Weight\":0,\"WeightUnit\":\"Pounds\",\"Width\":0,\"Height\":0,\"Depth\":0,\"DimensionsUnit\":\"Inches\",\"Status\":\"awaiting_shipment\",\"OtherOptions\":{\"BillToParty\":\"third_party\",\"BillToAccount\":\"X49188\",\"BillToPostalCode\":\"61236\",\"BillToCountryCode\":\"US\",\"BillToMyOtherAccount\":483738}},{\"ShippingAgentCode\":\"ups\",\"ShippingAgentService\":\"ups_ground\",\"PackageNo\":2,\"OrderId\":0,\"OrderKey\":\"\",\"SourceNo\":\"WHSESHIP-000222\",\"PackingDate\":\"2024-02-27T20:36:30.1770000Z\",\"CustomerUsername\":\"3rdAVEKITEREPAIR\",\"CustomerEmail\":\"diego.rozo@mscloudexperts.com\",\"BillTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSAPlur-eV3\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"},\"ShipTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSAPlur-eV3\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"},\"Lines\":[{\"PackageNo\":2,\"ItemNo\":\"K3KOSWTCH\",\"Name\":\"K3KOSWTCH\",\"QtyToHandle\":1,\"LineNo\":1000,\"SourceNo\":\"SOB2B-301734\",\"WarehouseDocumentNo\":\"WHSEPICK-00036\",\"WarehouseLineNo\":30000,\"VariantCode\":\"012011\",\"ItemPrice\":1469}],\"Weight\":0,\"WeightUnit\":\"Pounds\",\"Width\":0,\"Height\":0,\"Depth\":0,\"DimensionsUnit\":\"Inches\",\"Status\":\"awaiting_shipment\",\"OtherOptions\":{\"BillToParty\":\"third_party\",\"BillToAccount\":\"X49188\",\"BillToPostalCode\":\"61236\",\"BillToCountryCode\":\"US\",\"BillToMyOtherAccount\":483738}}]"
}
```

**Note:** `La documentacion de este request es lo mismo usando en la api creada para Plur-e Mobile` 
[Link](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/271/Shipstation)

**Response:** 

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "CreateOrUpdatePackageShipment",
    "userId": null,
    "result": "{\"HasErrors\":false,\"Results\":[{\"OrderId\":52677276,\"OrderNumber\":\"WHSESHIP-000223-1\",\"OrderKey\":\"d1368e3f20014c6a8aa134500797a595\",\"SourceNo\":\"WHSESHIP-000223\",\"PackageNo\":1,\"Success\":true,\"ErrorMessage\":null},{\"OrderId\":52677279,\"OrderNumber\":\"WHSESHIP-000223-2\",\"OrderKey\":\"1d5c35f624a74fcc9689cb9a094165af\",\"SourceNo\":\"WHSESHIP-000223\",\"PackageNo\":2,\"Success\":true,\"ErrorMessage\":null}]}",
    "error": ""
}
```