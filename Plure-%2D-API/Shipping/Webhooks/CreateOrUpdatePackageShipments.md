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
    "CustomerId": "cus_OTWT9NtE1HGhmP",
    "EnvironmentId": "env_278136d30f374d77b1881216b995f25f",
    "ProcessMethod": "CreateOrUpdatePackageShipment",
    "CompanyId": "d3a2f34b-de27-ee11-bdf5-6045bd828f66",
    "JsonRequest": "[{\"OrderId\":21035510,\"OrderKey\"cb584082dc2545d28721f39bc0cd9207:\"\",\"SourceNo\":\"WHSE SHIP-00030\",\"PackageNo\":4,\"PackingDate\":\"2023-09-26T21:54:20.3970000Z\",\"CustomerUsername\":\"Trey Research\",\"CustomerEmail\":\"helen.ray@contoso.com\",\"BillTo\":{\"Name\":\"Trey Research\",\"Company\":\"Adventure\",\"Address1\":\"153 Thomas Drive\",\"Address2\":\"\",\"City\":\"Chicago\",\"State\":\"IL\",\"Country\":\"US\",\"PostalCode\":\"61236\",\"Phone\":\"\"},\"ShipTo\":{\"Name\":\"Trey Research\",\"Company\":\"Adventure\",\"Address1\":\"153 Thomas Drive\",\"Address2\":\"\",\"City\":\"Chicago\",\"State\":\"IL\",\"Country\":\"US\",\"PostalCode\":\"61236\",\"Phone\":\"\"},\"Lines\":[{\"PackageNo\":1,\"ItemNo\":\"1900-S\",\"Name\":\"1900-S\",\"QtyToHandle\":2,\"LineNo\":1000,\"SourceNo\":\"S-ORD101046\",\"WarehouseDocumentNo\":\"WHSE PICK-00023\",\"WarehouseLineNo\":40000,\"VariantCode\":\"\"}],\"Weight\":8,\"WeightUnit\":2,\"Width\":8,\"Height\":8,\"Depth\":8,\"DimensionsUnit\":1,\"Status\":\"awaiting_shipment\"}]"
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