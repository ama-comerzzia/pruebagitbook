## Configuración de los parámetros del Sistema {#configuraci-n-de-los-par-metros-del-sistema}

Se trata de una pantalla de Administración de variables internas del sistema, que nos permitirá definir una configuración personalizada para nuestro sistema:

A continuación se detallan las variables configurables en el sistema:

### Variables configurables: Artículos {#variables-configurables-art-culos}

*   “Título para el primer desglose en almacén”
*   “Título para el segundo desglose en almacén”
*   &quot;Formato de los códigos de barras aleatorios&quot;

Los dos “niveles de desglose” son opcionales (Talla y Color para el ejemplo representado) y, en caso de decidir usarlos, son los nombres que dinámicamente recogerán las pantallas del sistema.

El formato de los códigos de barras aleatorios puede ser EAN13 o EAN18 (este último es el valor por defecto); los códigos de barras generados de forma aleatoria en el mantenimiento de artículos tendrán un formato u otro según la opción seleccionada.

### Variables configurables: Tarifas {#variables-configurables-tarifas}

*   Primer nivel de redondeo de tarifas. Desde/Hasta/Valor
*   Segundo nivel de redondeo de tarifas. Desde/Hasta/Valor
*   Tercer nivel de redondeo de tarifas. Desde/Hasta/Valor

Con estos parámetros se establece una **forma opcional de hacer redondeo**, sobre las dos primeras posiciones decimales de los precios (PVP+impuestos) en tarifa, en el proceso de “Actualización masiva de Artículos en la Tarifa”, descrito en apartado posterior de este manual, específico de proceso de Ventas y gestión de Tarifas.

Como podemos observar se establecen rango de valores desde/hasta y valor asignado para la posición decimal correspondiente.

### Variables configurables: POS {#variables-configurables-pos}

*   “Uso de descuentos en líneas para los tickets realizados por el POS”: es posible activar esta posibilidad de aplicar descuento a nivel de línea de detalle en los documentos de venta.
*   “Realizar la venta de artículos con precio 0”: posibilidad de activar o desactivar la opción que permite vender artículos con precio 0.
*   “Permitir el cambio de precio en edición”: posibilidad de modificar el precio de los artículos desde la pantalla de edición de línea.
*   “Para finalizar una venta la fecha de apertura de caja deberá ser igual a la fecha del sistema: Permite incorporar un control más en el proceso de venta para no poder hacer ventas en día diferente al de apertura de la caja.
*   “Realizar apertura automática de caja al entrar en las pantallas de venta”: Permite configurar la apertura automática de la caja al iniciar con el proceso de venta.
*   “Columna vendedor visible en la pantalla de ventas del POS”: Permite visualizar el vendedor asociado a cada línea de la pantalla de Ventas del POS.
*   “Aplicar promociones de precio antes que el resto, que se aplicarían sobre el precio promoción”: Permite configurar las promociones de forma que las promociones de precio de artículos se apliquen antes que el resto de promociones activas, aplicándolas a posteriori sobre el precio fijado en la promoción de precio y no sobre el de tarifa.
*   &quot;Número de reintentos para cerrar la caja con descuadres&quot;: Indicamos el número máximo de intentos que se permiten para poder cerrar la caja con descuadres.
*   Actualmente en desuso a partir de la V.3.x de comerzzia:
    *   _“Permitir devolver más cantidad del total de la devolución”: la selección de esta opción permitirá devolver un importe mayor que el total de la devolución. Actualmente en desuso a partir de la V.3.0 de comerzzia._
    *   _“Tener en cuenta las líneas de devolución en las promociones”: mediante esta opción se determinará si los artículos reflejados en un ticket son considerados para llevar a cabo el tratamiento de las promociones. Actualmente en desuso a partir de la V.3.0 de comerzzia._

### Variables configurables: Servicios REST {#variables-configurables-servicios-rest}

Indica la clave de acceso a los servicios REST de ComerZZia.