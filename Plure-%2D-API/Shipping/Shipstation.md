### Description
This is the model of the JSON that the API receive and send as response in order to create an order on Shipstation (SS)

**HTTP Method:** `Post`

**Endpoint:** `/api/v1.0/Shipments/create`

**Parameters:** 
- **SourceNo:** A user-defined order number used to identify an order.
- **PackingDate:** The date the order was placed.
- **CustomerUsername:** The customer's username. (SS: This property needs to be defined to generate a customer profile.)
- **CustomerEmail:** The customer's email address.
- **BillTo:** The recipient's billing address.
  - **Name:** Name of person.
  - **Company:** Name of the company
  - **Address1:** First Line of the address
  - **Address2:** Second Line of the address
  - **City:** City
  - **State:** State
  - **Country:**  Country Code. The [two-letter ISO Origin Country code](https://www.nationsonline.org/oneworld/country_code_list.htm) is required.
- **ShipTo:** The recipient's shipping address.
  - **Name:** Name of person.
  - **Company:** Name of the company
  - **Address1:** First Line of the address
  - **Address2:** Second Line of the address
  - **City:** City
  - **State:** State
  - **Country:** Country Code. The [two-letter ISO Origin Country code](https://www.nationsonline.org/oneworld/country_code_list.htm) is required.
  - **PostalCode:** Postal Code
  - **Phone:** 	Telephone number.
- **Lines:** An array of item objects.
  - **ItemNo:** The SKU (stock keeping unit) identifier for the product associated with this line item.
  - **Name:** The name of the product associated with this line item. Cannot be null
  - **QtyToHandle:** The quantity of product ordered.
  - **ProductId:** The identifier for the Product Resource associated with this item. (pending)
- **Weight:** Weight of package.
- **WeightUnit:** units of weight. Allowed units are: "pounds", "ounces", or "grams"
- **Width:** Width of package.
- **Height:** Height of package.
- **Depth:** Length of package.
- **DimensionsUnit:** Units of measurement. Allowed units are: "inches", or "centimeters"

## Example:

```
{
	"CustomerId": "cus_a87d98ad79asd",
	"EnvironmentId": "env_9ad9a0sd9asd",	
    "ProcessMethod": "CreateOrUpdatePackageShipment",
	"CompanyId": "1FE5E7A4-BB21-409E-BE72-55BD98E5C446",	
    "JsonRequest": [{
            "SourceNo": "S-ORD101011",
            "PackingDate": "2023-09-02T00:00:00.0000000",
            "CustomerUsername": "SportCenter",
            "CustomerEmail": "sport@sport.com",
            "BillTo": {
                "Name": "Pepa Perez",
                "Company": "Sport Center",
                "Address1": "192 Market Square",
                "Address2": "",
                "City": "Atlanta",
                "Country": "US",
                "State": "GA"
            },
            "ShipTo": {
                "Name": "Pepa Perez",
                "Company": "Sport Center",
                "Address1": "192 Market Square",
                "Address2": "",
                "City": "Atlanta",
                "Country": "US",
                "State": "GA",
                "PostalCode": "30030",
                "Phone": "8973561324"
            },
            "Lines": [{
                    "ItemNo": "1896-S",
                    "Name": "ATHENS Desk",
                    "QtyToHandle": 1
                }, {
                    "ItemNo": "1908-S",
                    "Name": "ATHENS Desk",
                    "QtyToHandle": 3
                }
            ],
            "Weight": 1000.0,
            "WeightUnit": "grams",
            "Width": 28.0,
            "Height": 3.0,
            "Depth": 4.0,
            "DimensionsUnit": "centimeters",
            "Status": false,
            "SystemCreatedAt": "2023-07-28T15:55:58.9600000Z",
            "SystemCreatedBy": "{37E91226-6B8A-47A8-A580-E714FC6BFB7E}"
        }
    ]
}

```

## Response:

this will be an array of JSON with each order response 

## Example:

```
{
    "hasErrors": false,
    "results": [
        {
            "orderId": 17086108,
            "orderNumber": "S-ORD101011",
            "orderKey": "ee72417e259c4450ababefec1ddfca50",
            "success": true,
            "errorMessage": null
        },
        {
            "orderId": 17086110,
            "orderNumber": "S-ORD101012",
            "orderKey": "4f2a80ea1cf84d779f67e0eb9b58d63e",
            "success": true,
            "errorMessage": null
        }
    ]
}
```

