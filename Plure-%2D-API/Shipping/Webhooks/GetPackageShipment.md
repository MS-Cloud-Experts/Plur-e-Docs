### Description
Esta API permite obtener los Shipments transactions que se han realizado atraves de plur-e

**HTTP Method:** `Post`

**Endpoint:** `api/v1.0/webhooks?appSource=erp&customerId={customerId}&parms={parms}&secretKey={secretKey}`
#### Example:
```
api/v1.0/webhooks?appSource=erp&customerId=cus_OvXEmIZPtOMjoo&parms=WTNWelgwOTJXRVZ0U1ZwUWRFOU5hbTl2c2tfTnpnNVltRTJZbVV0T0RnME9TMDBZbVE1TFRsaU9UVXRNREprTURjMk9UUTFPREF6&secretKey=sk_Nzg5YmE2YmUtODg0OS00YmQ5LTliOTUtMDJkMDc2OTQ1ODAz
``` 

Esta api permite realizar dos tipos de consultas.

1. Consultar varios shipment transactions segun un rango de fecha, el request se debe enviar de la siguiente forma:

**Request:** 

```
{
    "CustomerId": "cus_OvXEmIZPtOMjoo",
    "EnvironmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "CompanyId": "BEBA99E4-2A78-EE11-817A-002248A527C3",
    "ProcessMethod": "GetPackageShipment",
    "JsonRequest": "{\"OrderId\":0,\"ForceUpdate\":true,\"FromDate\":\"2024-01-15\",\"ToDate\":\"2024-01-15\"}"    
}
```

**Response:** 

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "GetPackageShipment",
    "userId": null,
    "result": "[{\"ShipingOrderId\":\"0b2b7e1e-f618-4055-a515-6fc847927d9a\",\"CustomerId\":\"cus_OvXEmIZPtOMjoo\",\"EnvironmentId\":\"env_6b23fc1a48c046d4b6f4504d876ffeab\",\"CompanyId\":\"beba99e4-2a78-ee11-817a-002248a527c3\",\"OrderId\":43088959,\"OrderKey\":\"beb981fa54374bc79d2c3eea5e441397\",\"OrderNumber\":\"WHSEPICK-00092-1\",\"OrderStatus\":\"awaiting_shipment\",\"CarrierCode\":\"ups_walleted\",\"ServiceCode\":\"ups_ground_saver\",\"PackageCode\":null,\"TrackingNumber\":null,\"ShipmentCost\":0.00,\"ShipDate\":\"0001-01-01T00:00:00\",\"Items\":null,\"CreatedOn\":\"2024-01-16T14:06:24.4866531\",\"ModifiedOn\":\"2024-01-16T14:06:24.5067233\",\"VoidDate\":\"0001-01-01T00:00:00\",\"Voided\":false,\"OrderDate\":\"2024-01-15T08:26:09.837\",\"Carrier\":null,\"Submitted\":false,\"SubmittedDate\":\"0001-01-01T00:00:00\"},{\"ShipingOrderId\":\"71b38afe-7453-4d24-8ef7-28529bc0dcc5\",\"CustomerId\":\"cus_OvXEmIZPtOMjoo\",\"EnvironmentId\":\"env_6b23fc1a48c046d4b6f4504d876ffeab\",\"CompanyId\":null,\"OrderId\":43092845,\"OrderKey\":\"78a11cc7cbad496d9f222bf319a3d65f\",\"OrderNumber\":\"WHSE PICK-00092-1\",\"OrderStatus\":\"awaiting_shipment\",\"CarrierCode\":\"ups_walleted\",\"ServiceCode\":\"ups_ground_saver\",\"PackageCode\":null,\"TrackingNumber\":null,\"ShipmentCost\":0.00,\"ShipDate\":\"0001-01-01T00:00:00\",\"Items\":null,\"CreatedOn\":\"2024-01-16T19:18:49.539268\",\"ModifiedOn\":\"2024-01-16T19:18:49.5392699\",\"VoidDate\":\"0001-01-01T00:00:00\",\"Voided\":false,\"OrderDate\":\"2024-01-15T08:26:09.837\",\"Carrier\":null,\"Submitted\":false,\"SubmittedDate\":\"0001-01-01T00:00:00\"},{\"ShipingOrderId\":\"b10ea338-c04d-4702-8ea6-24e182ec7b2e\",\"CustomerId\":\"cus_OvXEmIZPtOMjoo\",\"EnvironmentId\":\"env_6b23fc1a48c046d4b6f4504d876ffeab\",\"CompanyId\":\"beba99e4-2a78-ee11-817a-002248a527c3\",\"OrderId\":43091416,\"OrderKey\":\"761fd1c542a94eff899ff76d1523f40e\",\"OrderNumber\":\"WHSEPICK-00192-1\",\"OrderStatus\":\"awaiting_shipment\",\"CarrierCode\":\"ups_walleted\",\"ServiceCode\":\"ups_ground_saver\",\"PackageCode\":null,\"TrackingNumber\":null,\"ShipmentCost\":0.00,\"ShipDate\":\"0001-01-01T00:00:00\",\"Items\":null,\"CreatedOn\":\"2024-01-16T19:14:01.4317702\",\"ModifiedOn\":\"2024-01-16T19:14:01.4317739\",\"VoidDate\":\"0001-01-01T00:00:00\",\"Voided\":false,\"OrderDate\":\"2024-01-15T08:26:09.837\",\"Carrier\":null,\"Submitted\":false,\"SubmittedDate\":\"0001-01-01T00:00:00\"}]",
    "error": ""
}
```

2. consultar por un shipment transaction en particular, el request se debe enviar de la siguiente forma:

**Request**
```
{
    "CustomerId": "cus_OvXEmIZPtOMjoo",
    "EnvironmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "CompanyId": "BEBA99E4-2A78-EE11-817A-002248A527C3",
    "ProcessMethod": "GetPackageShipment",
    "JsonRequest": "{\"OrderId\":43088959,\"ForceUpdate\":true,\"FromDate\":\"\",\"ToDate\":\"\"}"
}
```
**Response:** 

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "GetPackageShipment",
    "userId": null,
    "result": "[{\"ShipingOrderId\":\"0b2b7e1e-f618-4055-a515-6fc847927d9a\",\"CustomerId\":\"cus_OvXEmIZPtOMjoo\",\"EnvironmentId\":\"env_6b23fc1a48c046d4b6f4504d876ffeab\",\"CompanyId\":\"beba99e4-2a78-ee11-817a-002248a527c3\",\"OrderId\":43088959,\"OrderKey\":\"beb981fa54374bc79d2c3eea5e441397\",\"OrderNumber\":\"WHSEPICK-00092-1\",\"OrderStatus\":\"awaiting_shipment\",\"CarrierCode\":\"ups_walleted\",\"ServiceCode\":\"ups_ground_saver\",\"PackageCode\":null,\"TrackingNumber\":null,\"ShipmentCost\":0.00,\"ShipDate\":\"0001-01-01T00:00:00\",\"Items\":null,\"CreatedOn\":\"2024-01-16T14:06:24.4866531\",\"ModifiedOn\":\"2024-01-16T14:06:24.5067233\",\"VoidDate\":\"0001-01-01T00:00:00\",\"Voided\":false,\"OrderDate\":\"2024-01-15T08:26:09.837\",\"Carrier\":null,\"Submitted\":false,\"SubmittedDate\":\"0001-01-01T00:00:00\"},{\"ShipingOrderId\":\"0b2b7e1e-f618-4055-a515-6fc847927d9a\",\"CustomerId\":\"cus_OvXEmIZPtOMjoo\",\"EnvironmentId\":\"env_6b23fc1a48c046d4b6f4504d876ffeab\",\"CompanyId\":\"beba99e4-2a78-ee11-817a-002248a527c3\",\"OrderId\":43088959,\"OrderKey\":\"beb981fa54374bc79d2c3eea5e441397\",\"OrderNumber\":\"WHSEPICK-00092-1\",\"OrderStatus\":\"awaiting_shipment\",\"CarrierCode\":\"ups_walleted\",\"ServiceCode\":\"ups_ground_saver\",\"PackageCode\":null,\"TrackingNumber\":null,\"ShipmentCost\":0.00,\"ShipDate\":\"0001-01-01T00:00:00\",\"Items\":null,\"CreatedOn\":\"2024-01-16T14:06:24.4866531\",\"ModifiedOn\":\"2024-01-16T14:06:24.5067233\",\"VoidDate\":\"0001-01-01T00:00:00\",\"Voided\":false,\"OrderDate\":\"2024-01-15T08:26:09.837\",\"Carrier\":null,\"Submitted\":false,\"SubmittedDate\":\"0001-01-01T00:00:00\"}]",
    "error": ""
}
```
