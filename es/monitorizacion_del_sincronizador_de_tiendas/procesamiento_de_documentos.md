## Procesamiento de Documentos {#procesamiento-de-documentos}

Para poder ejecutar el procesado de documentos es necesario que el “Procesador de Datos” esté en funcionamiento.

La supervisión de todos los trabajos de procesado de documentos provenientes de las Tiendas se realiza desde el menú **“Almacén-Tienda”-&gt;Procesamiento de Documentos.**

En caso de que al acceder a este elemento de menú aparezca el siguiente mensaje, será necesario arrancar los servicios de “Sincronizador y/o Procesador de Datos” desde el menú de **“Sistema”**:

### Qué supone el procesado de Documentos en Comerzzia 3.x {#qu-supone-el-procesado-de-documentos-en-comerzzia-3-x}

Elprocesado de documentos en comerzzia 3.x supone un concepto más amplio que un simple documento de venta.

Es por ello que existe el concepto **“Tipo de Documento”** mediante el que se identificará el tipo de documento procesado. Como tipo de documento estarán:

*   Los **documentos de venta** parametrizados y que sea posible generar desde cada tienda, en función de su país de pertenencia. En la actualidad, se procesan las facturas simplificadas, facturas completas, notas de crédito así como los tipos de documentos de venta específicos de los países contemplados en la internacionalización de ComerZZia. Para más información, consultar los manuales de Internacionalización por países. Los diferentes tipos de documentos de venta disponibles en comerzzia 3.0 son:
    *   Ventas por cliente: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por cliente.
    *   Ventas por familias: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por familia.
    *   Ventas por artículos: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por artículo.
*   Los **cierres de caja** que, a partir de ComerZZia 3.0, quedan englobados en este concepto. Los informes de cierres de caja disponibles en comerzzia son:
    *   Cierre de caja totalizado: Muestra todos los cierres de caja que se han hecho por cada día, tienda y caja. En cada uno de ellos indica el total teórico, el total contado, y el descuadre entre ambos.
    *   Cierre de caja detallado: Muestra lo mismo que el anterior, pero desglosado por cada forma de pago.
    *   Movimientos de caja totalizados: Muestra, en el rango de fechas indicado, por cada tienda y caja, todos los apuntes de caja manuales (salida de efectivo, retirada de caja, etc.) agrupados por concepto.
    *   Movimientos de caja detallados: Muestra lo mismo que el anterior, pero desglosado por cada día dentro del rango de fechas seleccionado.
*   Este concepto es ampliable a futuro a **otros tipos de documentos** que sea necesario procesar por el sistema, no necesariamente asociados a la venta.

El procesado de un documento supone el alta/inserción en el sistema de dicho documento, quedando asociado a:

*   La Serie de la Tienda que lo ha generado.
*   El Almacén asociado a la tienda que lo ha generado.
*   El Cliente con el que se realizó la venta (genérico de la tienda o específico)
    *   El documento de venta hace referencia al Cliente a través del tipo de documento y número de identificación asociado. Si en el sistema no existe Cliente con el nº identificativo indicado en el ticket, la aplicación dará de alta, de forma automática, un nuevo Cliente con tipo de documento y código igual al especificado en el documento de venta.
*   El Concepto de Almacén de Venta será el Concepto especificado para la Tienda.

### Listado de Documentos pendientes de procesar {#listado-de-documentos-pendientes-de-procesar}

Presenta los documentos pendientes de procesar, agrupados por fecha y tienda

### Listado de Tickets Procesados {#listado-de-tickets-procesados}

Presenta los documentos procesados, agrupados por fecha y tienda, permitiendo establecer criterio de búsqueda por rango de fechas y Tienda:

### Listado de Documentos Erróneos {#listado-de-documentos-err-neos}

Presenta los documentos con errores en el procesado, agrupados por fecha y tienda, permitiendo establecer criterio de búsqueda por rango de fechas y Tienda, e informando de la fecha del proceso y tipo de problema

Sobre esta pantalla podemos realizar las siguientes acciones:

: Consultar y Editar el documento seleccionado

: Borrar el documento seleccionado

: Volver a procesar el documento seleccionado

: Volver a procesar todos los documentos.