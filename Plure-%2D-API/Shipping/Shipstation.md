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
  - **Country:**  Country Code. The [two-letter ISO Origin Country code](https://www.nationsonline.org/oneworld/country_code_list.htm) is required.
- **ShipTo:** The recipient's shipping address.
  - **Name:** Name of person.
  - **Company:** Name of the company
  - **Address1:** First Line of the address
  - **Address2:** Second Line of the address
  - **City:** City
  - **Country:** Country Code. The [two-letter ISO Origin Country code](https://www.nationsonline.org/oneworld/country_code_list.htm) is required.
- **Lines:** An array of item objects.
  - **ItemNo:** The SKU (stock keeping unit) identifier for the product associated with this line item.
  - **Name:** The name of the product associated with this line item. Cannot be null
  - **QtyToHandle:** The quantity of product ordered.
  - **ProductId:** The identifier for the Product Resource associated with this item.
- **Weight:** Weight of package.
- **WeightUnit:** units of weight. Allowed units are: "pounds", "ounces", or "grams"
- **Width:** Width of package.
- **Height:** Height of package.
- **Depth:** Length of package.
- **DimensionsUnit:** Units of measurement. Allowed units are: "inches", or "centimeters"

## Example:




