### Description
Esta API permite eliminar los Shipments transactions que se han realizado atraves de plur-e

**HTTP Method:** `Post`

**Endpoint:** `api/v1.0/webhooks?appSource=erp&customerId={customerId}&parms={parms}&secretKey={secretKey}`
#### Example:
```
api/v1.0/webhooks?appSource=erp&customerId=cus_OvXEmIZPtOMjoo&parms=WTNWelgwOTJXRVZ0U1ZwUWRFOU5hbTl2c2tfTnpnNVltRTJZbVV0T0RnME9TMDBZbVE1TFRsaU9UVXRNREprTURjMk9UUTFPREF6&secretKey=sk_Nzg5YmE2YmUtODg0OS00YmQ5LTliOTUtMDJkMDc2OTQ1ODAz
``` 
****Criterios****
#### CustomerId: 
Id del cliente asignado al momento de crear la subscripcion
#### EnvironmentId: 
Id del environment asignado al ambiente instalado
#### CompanyId: 
Id de la compañia 
#### ProcessMethod: 
Se debe enviar *****DeletePackageShipment*****
#### JsonRequest: 
Este criterio es muy importante, aqui se debe enviar el listado de OrderIds a eliminar, acontinuacion la explicacion de la estructura que se debe enviar:

```
[{\"OrderId\":0},{\"OrderId\":1},...,{\"OrderId\":n}]
```


###----------------------------------------------------------------------------------------------------------------------------------------

Esta api permite eliminar una o muchas ordenes de shipstation:

1. Eliminar una orden, el request se debe enviar de la siguiente forma:

**Request:** 

```
{
    "CustomerId": "cus_OvXEmIZPtOMjoo",
    "EnvironmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "CompanyId": "BEBA99E4-2A78-EE11-817A-002248A527C3",
    "ProcessMethod": "GetPackageShipment",
    "JsonRequest": "[{\"OrderId\":0}]"    
}
```

**Response:** 

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "DeletePackageShipment",
    "userId": null,
    "result": "[{\"OrderId\":52484156,\"Success\":true,\"Message\":\"The requested order has been deleted.\"},{\"OrderId\":52484157,\"Success\":true,\"Message\":\"The requested order has been deleted.\"}]",
    "error": ""
}
```
**Exeptions:**

En caso de ocurra algun error en shipstation o el OrderId no sea encontrado, recibira la razon del error en la propiedad result, acontinuacion un ejemplo de como se ve un error:

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "DeletePackageShipment",
    "userId": null,
    "result": "[{\"OrderId\":52484156,\"Success\":false,\"Message\":\"Shipping order Id 52484156, not found.\"},{\"OrderId\":52484157,\"Success\":false,\"Message\":\"Shipping order Id 52484157, not found.\"}]",
    "error": ""
}
```

Otro tipo de error que puede ocurrir son los errores internos de Plur-e API, estos mensajes de error llegaran de la siguiente forma:

```
{
    "customerId": "cus_OvXEmIZPtOMjoo",
    "environmentId": "env_6b23fc1a48c046d4b6f4504d876ffeab",
    "processMethod": "DeletePackageShipment",
    "userId": null,
    "result": null,
    "error": "Could not convert string to integer: ssssss. Path '[0].OrderId', line 1, position 20."
}
```