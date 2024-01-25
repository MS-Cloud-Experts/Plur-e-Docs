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
    "companyId": "beba99e4-2a78-ee11-817a-002248a527c3",
    "jsonRequest": "[{\"PackageNo\":1,\"SourceNo\":\"WHSEPICK-00192\",\"WarehouseDocumentNo\":\"WHSEPICK-00092\",\"WarehouseShipmentNo\":\"WHSESHIP-00087\",\"CustomerUsername\":\"3rdAVEKITEREPAIR\",\"CustomerEmail\":\"diego.rozo@mscloudexperts.com\",\"WeightUnit\":\"Pounds\",\"DimensionsUnit\":\"Inches\",\"Status\":\"awaiting_shipment\",\"OrderId\":0,\"OrderKey\":\"\",\"Weight\":0.0,\"Width\":0.0,\"Height\":0.0,\"Depth\":0.0,\"TotalQty\":10.0,\"Release\":true,\"RegisteredPick\":\"\",\"PackageTrackingNo\":\"\",\"ShippingAgentCode\":\"ups_walleted\",\"ShippingAgentService\":\"ups_ground_saver\",\"PackingDate\":\"2024-01-15T16:26:09.8370000Z\",\"ShippingDate\":\"0001-01-01\",\"Lines\":[{\"PackageNo\":1,\"LineNo\":1000,\"SourceNo\":\"SOB2B-300820\",\"SourceLineNo\":10000,\"WarehouseDocumentNo\":\"WHSEPICK-00092\",\"WarehouseLineNo\":10000,\"ItemNo\":\"D0AVESVTBLU00S\",\"VariantCode\":\"\",\"SerialNo\":\"\",\"LotNo\":\"\",\"QtyToHandle\":10}],\"ShipTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSA-PLUR-EV2\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"},\"BillTo\":{\"Name\":\"3rdAVEKITEREPAIR\",\"Company\":\"AdventureSportsUSA-PLUR-EV2\",\"Address1\":\"370BODEGAST\",\"Address2\":\"\",\"City\":\"FosterCity\",\"State\":\"California\",\"Country\":\"US\",\"PostalCode\":\"94404\",\"Phone\":\"16505207654\"}}]"
}
```


**Note:** `La documentacion de este request es lo mismo usando en la api creada para Plur-e Mobile` 
****[Link](https://dev.azure.com/MSCloudExperts/Plur-e/_wiki/wikis/Plur-e.wiki/271/Shipstation)****

**Response:** 

```
{
    "customerId": "cus_OTWT9NtE1HGhmP",
    "environmentId": "env_278136d30f374d77b1881216b995f25f",
    "processMethod": "CreateOrUpdatePackageShipment",
    "userId": null,
    "result": "{\"HasErrors\":false,\"Results\":[{\"OrderId\":21035510,\"OrderNumber\":\"WHSE SHIP-00030-4\",\"OrderKey\":\"cb584082dc2545d28721f39bc0cd9207\",\"Success\":true,\"ErrorMessage\":null}]}",
    "error": ""
}
```