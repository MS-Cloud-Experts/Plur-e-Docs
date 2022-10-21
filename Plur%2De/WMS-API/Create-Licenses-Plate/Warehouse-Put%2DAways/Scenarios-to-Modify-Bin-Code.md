**Scenarios:**

1) **There are only LP Singles, there are no LP Pallets.**

![image.png](/.attachments/image-6550fa7e-a576-441e-ae1b-4ae261159d9e.png)

Solution: 
   Call the method **Prepare_WarehousePutAway** and then 
    **Update_WarehousePutAway_Lines** with the **Bin** of the **LP** you want to Update.

2) **Change the destination Bin of all the Put-Away.**

Before
![imagen.png](/.attachments/imagen-1d9556d3-64fb-4e57-ac5a-12946a9c5272.png)

After

![imagen.png](/.attachments/imagen-e3df2d6d-b2e0-49fb-bfaa-b768a1ef3fc9.png)

**Solution**: Only **Update_Wsheput_Lines_V2** will be called, and the information will be obtained from the **Warehouse Put Away Lines**


3) **Change the destination Bin of an LP Pallet with only Items as children**
4) **Change the Destination Bin of an LP Pallet with only LP Singles as children**
5) **Change the destination Bin of a mixed LP Pallet, LP, and Items as children.**