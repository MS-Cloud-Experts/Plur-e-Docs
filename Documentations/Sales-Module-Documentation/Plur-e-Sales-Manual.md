# Plur e Sales Manual

## 1. INTRODUCTION
Plur-E is a sales application integrated with Business Central

- Users must have:
  - Sales-related permissions in Business Central
  - Be listed in the Salespeople/Purchasers window

## **2. SALES ORDERS**

###**Creating Sales Order with Partial Shipment**

1. Create SO from Plur-e Mobile
2. Add items by:
   - Manual entry
   - Scanning function
3. Select for each item:
   - Location
   - Unit of measure
   - Quantity (can increase/decrease)
4. Use picking function
   - Assign different quantities for partial shipment
5. Validate creation in Business Central

**Create Sales Order in Plur-e Mobile**

- Access the Plur-e Mobile application
- Navigate to the "Sales Orders" section
- Click on "New Sales Order" button
- Select or verify the customer information
- Choose delivery address and billing details
- Set the desired delivery date

**Adding Items to the Order**

Manual Entry Method:

Click on "Add Item" or similar button

- Search for products using:

Product code
Product name
Product category

- Select the desired item from the search results
- Verify product details before adding

Scanning Function Method

- Click on the scan button or barcode icon
- Position the camera to read the product barcode
- Verify that the scanned product is correct
- Confirm the addition to the order

**Item Configuration**

For each product in the order:

Location Selection:

- Choose the warehouse location
- Verify stock availability at selected location
- Confirm the picking location

Unit of Measure Settings:

- Select appropriate unit of measure
- Verify the conversion rates if applicable
- Confirm unit pricing

Quantity Configuration:

- Enter the total quantity needed
- Verify against available stock
- Confirm total amount matches customer request

**Picking Process**

Initial Setup:

Access the picking function
Verify order details
Confirm picking location


Quantity Assignment:

Assign full quantities for each item
Verify stock availability
Ensure picking quantities match order quantities


Picking Confirmation:

Review all assigned quantities
Confirm complete picking list
Generate picking documentation



5. Business Central Validation

Order Review:

Check all item details
Verify pricing and discounts
Confirm shipping information


Document Generation:

Create necessary shipping documents
Generate packing lists
Prepare delivery documentation


Final Validation:

Verify all quantities match
Confirm complete shipment details
Approve order in Business Central

###**Creación de Orden de Venta con Envío Completo**

**Inicio de la Orden**

- Abre Plur-e Mobile
- Dirigirte a la sección de "Sales Orders"
- Selecciona "Crear Nueva Orden de Venta", el sistema abrirar una pestaña nueva donde podras configurar la orden de venta nueva.

**Agregar Productos**

Entrada Manual:

- Busca el producto por nombre o código y selecciona del catálogo

Función de Escaneo:

- Usa el escáner para leer códigos de barras, este escáner en un celular es la camara del mismo, si es un dispositivo Zebra este vendrá equipado con un lector de codigo de barras.
- Verifica que el producto escaneado sea correcto

**Configuración de Items**

Para cada producto debes especificar:

- Selecciona la ubicación del almacén
- Elige la unidad de medida correcta
- Ingresa la cantidad total que se enviará
- Asegúrate de que las cantidades coincidan con el stock disponible


**Proceso de Picking**

A diferencia del envío parcial:

- Asigna la cantidad completa para cada ítem
- Verifica que las cantidades de picking coincidan con las cantidades ordenadas
- No dividas las cantidades ya que se enviará todo junto


**Validación Final**

- Revisa que todas las cantidades estén correctas
- Confirma que la ubicación de envío sea la adecuada
- Verifica los detalles del cliente
- Valida la orden en Business Central


**Confirmación del Envío**

- Genera el documento de envío
- Asegúrate de que todas las cantidades estén al 100%
- Confirma el envío completo

###**Diferencias clave con el envío parcial y Recomendaciones**

- No necesitas dividir cantidades
- Todas las cantidades deben coincidir con la orden original
- El picking se realiza en una sola operación
- La validación es más directa ya que no hay que controlar múltiples envíos
- Verifica el stock disponible antes de crear la orden
- Asegúrate de que todos los productos estén en la ubicación indicada
- Confirma que tienes capacidad de envío para todo el pedido
- Documenta cualquier incidencia durante el proceso


## 3. SALES RETURN ORDERS
1. Create new return order
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 4. SALES INVOICES
1. Create new sales invoice
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 5. SALES CREDIT MEMOS
1. Create new credit memo
2. Select customer
3. Add items
4. For each item:
   - Select location
   - Choose unit of measure
   - Set quantity
5. Verify in Business Central

## 6. POST-CREATION OPERATIONS

6.1 Posting Documents
- Can post:
  - Sales orders
  - Return orders
  - Invoices
  - Credit memos

6.2 Posted Invoices
- View posted invoices
- Print posted invoices


IMPORTANT NOTES
- All document types follow similar attachment and printing procedures
- Verification in Business Central is required for all transactions
- Payment batch configuration is essential for processing payments
