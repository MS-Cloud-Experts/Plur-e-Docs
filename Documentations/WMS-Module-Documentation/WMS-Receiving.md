#**WMS Receiving Module**


##**1. Receiving in Plur-e Mobile:**

**Receiving Items**

   - Open the Warehouse Receipt section in the PLUR-E app.
   - Assign the user ID on the mobile device so that the orders are displayed.
   - Enter the Receipt submodule to view the created orders.
   - Select or scan the items to be received, entering the respective quantities and sending the data.

**Receiving Serialized Items**
   - Scan serial numbers individually and record quantities to ensure inventory accuracy.
   - If serial numbers are preloaded from an order, simply verify the data.

**Put-Away Process (Location Assignment)**
   - When receiving items, choose whether you want to proceed with the put-away process.
   - If you choose to continue, enter the quantities and select the destination Bin Code.
   - Move items to specific locations or apply changes to all items in bulk.

----
##**2. Receiving in Business Central:**

- Despues de crear la Purchase Order en Business Central, toca pulsar el botón "Create Warehouse Receipt", con el cual el sistema generara un documento de Warehouse Receipt, desde el cual podremos recivir las cantidades de los items que se pidieron en la Parchase Order.

- Ya en el Warehouse Receipt, se deberan llenar las cantidades a recibir (**Qty To Receive**) de los items que esten el documento, (**Nota:** si el item es manejado por plur-e, la manera de recibirlo es mediente las funcionalidades de License Plate).

- Una ves la cantidades registradas se debera postear el documento de Warehouse Receip mediente el boton **"Post Receipt"**
