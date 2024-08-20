### Pruebas Unitarias - Escenario de Transferencia de License Plates (LP) de Bin a Bin

#### **Propósito**
El objetivo de esta prueba es verificar el proceso de transferencia de License Plates (LP) de un bin a otro dentro del almacén utilizando la API `MoveBinToBinLP`. Esta prueba asegura que los LPs se muevan correctamente de un bin a otro, que las validaciones se realicen de manera adecuada, y que la integridad de los datos se mantenga durante todo el proceso.

#### **Preparación**

1. **Validación Previa**
   - **Acción**: Accede al almacén en Business Central y verifica que existan LPs en los bins de origen y destino que serán utilizados en la prueba.
   - **Verificación**: Confirma que los LPs estén en un estado adecuado para ser movidos, específicamente en estado "Stored", y que los bins de origen y destino estén correctamente configurados.

#### **Flujo de la Prueba**

2. **Validación de Ubicaciones y Bins**
   - **Propósito**: Asegurar que las ubicaciones y los bins seleccionados para la transferencia sean correctos.
   - **Acción**: Verifica que el bin de origen y el bin de destino sean diferentes, y que el bin de destino sea adecuado para el tipo de ítem almacenado en el LP.
   - **Verificación**: Asegúrate de que el sistema detecte cualquier inconsistencia, como un bin de origen igual al bin de destino, y genere la advertencia o error correspondiente.

3. **Ejecución de la API `MoveBinToBinLP`**
   - **Propósito**: Validar la correcta transferencia de los LPs entre bins.
   - **Acción**: Utiliza la API `MoveBinToBinLP` con los siguientes parámetros:
     - **ProcessMethod**: "MoveBinToBinLP"
     - **Parameters**: JSON array que contiene la lista de LPs a mover, por ejemplo:
       ```json
       {
         "ProcessMethod": "MoveBinToBinLP",
         "Parameters": [
           {
             "LPToMove": [
               {
                 "LPDocumentNo": "LP001",
                 "FromBin": "BIN-01",
                 "ToBin": "BIN-02"
               },
               {
                 "LPDocumentNo": "LP002",
                 "FromBin": "BIN-01",
                 "ToBin": "BIN-03"
               }
             ]
           }
         ]
       }
       ```
   - **Verificación**: Confirma que la respuesta de la API sea exitosa y que los LPs se hayan movido correctamente a los bins de destino especificados. Asegúrate de que no se presenten errores durante el proceso.

4. **Verificación de Movimientos en LP Movements**
   - **Propósito**: Garantizar que los movimientos de los LPs se registren correctamente.
   - **Acción**: Revisa la tabla `PLU LP Movements` para verificar que se han registrado dos movimientos por cada LP:
     - Un movimiento negativo en el bin de origen, reflejando la salida del LP.
     - Un movimiento positivo en el bin de destino, reflejando la entrada del LP.
   - **Verificación**: Asegúrate de que los movimientos estén registrados correctamente y que las cantidades y ubicaciones sean coherentes con la operación realizada.

5. **Verificación del Estado del LP**
   - **Propósito**: Asegurar que el estado del LP se haya actualizado correctamente después de la transferencia.
   - **Acción**: Verifica en la tabla `PLU LP New Headers` que el estado del LP permanezca en "Stored" después de la transferencia, indicando que el LP ha sido movido exitosamente a su nuevo bin.
   - **Verificación**: Confirma que el estado y bin del LP se han actualizado correctamente y que no hay inconsistencias.

#### **Escenarios Adicionales y Variantes**

6. **Transferencia de Múltiples LPs**
   - **Propósito**: Verificar que el sistema maneje correctamente la transferencia de múltiples LPs en una sola operación.
   - **Acción**: Realiza la misma prueba con varios LPs movidos desde y hacia diferentes bins.
   - **Verificación**: Asegúrate de que todos los LPs se muevan correctamente y que cada movimiento se registre sin errores.

7. **Escenario con LPs en Estados No Permitidos**
   - **Propósito**: Verificar el comportamiento del sistema cuando se intenta mover un LP en un estado no permitido, como "Blocked" o "Reserved".
   - **Acción**: Intenta mover un LP que esté en un estado incompatible con la transferencia.
   - **Verificación**: Confirma que el sistema genera un error y no permite la transferencia del LP, manteniendo la integridad del inventario.

#### **Conclusión**
Este plan de pruebas asegura una cobertura detallada del proceso de transferencia de LPs entre bins, validando cada paso y confirmando que el sistema maneja correctamente todas las operaciones y escenarios posibles. Implementar estas pruebas ayuda a garantizar que las operaciones de transferencia se realicen de manera eficiente, precisa y segura dentro del sistema de Business Central.