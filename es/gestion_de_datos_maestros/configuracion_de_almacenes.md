## Configuración de Almacenes {#configuraci-n-de-almacenes}

### Mantenimiento de Almacenes {#mantenimiento-de-almacenes}

Desde este punto de menú se podrán gestionar los almacenes de la empresa, tanto los que estén en la/s tienda/s como los que se encuentren en otra Ubicación.

Para listar los almacenes se deberá pulsar el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código y Descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Almacén:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

Desde este punto de menú se darán de alta los almacenes de la empresa, tanto los que estén en la/s tienda/s como los que se encuentren en otra Ubicación.

Aunque es conveniente rellenar todos los campos, los únicos campos obligatorios son el código, la descripción y la empresa.

Los campos de la pantalla son los siguientes:

*   Empresa: Empresa a la que se encuentra asociado el almacén.
*   Cliente: cada almacén debe tener asociado un cliente, de forma que cuando se hagan operaciones entre almacenes, por ejemplo, peticiones de una tienda, devoluciones o traspasos entre almacenes, se utilizará el cliente asociado al almacén para realizar la operación y se usará la tarifa de ese cliente. Cuando se da de alta un almacén, si no se rellena el campo cliente, al aceptar para grabar el registro, la aplicación preguntará si se desea crear un cliente automáticamente con los datos del almacén:
*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: nombre identificativo del almacén.
*   Domicilio, Población, Provincia, Código Postal: correspondientes a la ubicación física del almacén
*   Teléfonos y Fax
*   Persona de Contacto

### Mantenimiento de Tiendas {#mantenimiento-de-tiendas}

En la opción de menú de Mantenimiento de Tiendas podrán listarse todas las tiendas pulsando el botón “**Consultar”.**

También es posible filtrar la consulta por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Tienda:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera. También será posible dar de alta tiendas a través del asistente, tal y como se comenta en el apartado siguiente de este manual.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

Desde este punto de menú se darán de alta las tiendas de la empresa, entendiendo por Tienda como los diferentes establecimientos que existen con venta al público.

Los campos de la pantalla son los siguientes:

*   **Pestaña General**

**Datos de la Tienda:**

*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: Nombre de la Tienda.
*   Activo: si está en uso.
*   Datos de Contacto:
    *   **Cliente:** la tienda debe existir como Cliente, de forma que en las operaciones entre tiendas se utilizará ese cliente. Si al crear una tienda no se rellena el campo Cliente, la aplicación preguntará si se desea que se cree el registro automáticamente:
    *   **Empresa:** Empresa a la que se encuentra asociada la tienda.
    *   **Otros datos: Persona de contacto, domicilio, población, provincia, código postal, teléfonos y fax.**
*   Datos por defecto para la venta: cada tienda deberá tener asociado un **Concepto de Almacén**, que se usará en los documentos generados a partir de las ventas de las tiendas; un **Medio de Pago** para las ventas que se realicen en la tienda; también otros dos medios de pago para **Apartados** y **Promociones**, los cuales serán usados por el POS en apartados y promociones (consultar el manual del POS para más información sobre apartados y promociones). Al dar de alta la tienda se creará automáticamente un almacén con el mismo código que la tienda.
*   Tipo de Tienda: los tipos de tienda son:
    *   Online: trabaja directamente con los datos de la central
    *   Offline: tiene su propia base de datos, y por lo tanto requiere de procesos de sincronización. Los métodos de sincronización disponibles definirán los tipos de tienda y se explican en detalle en este manual.
*   Versión de artículos: ofrece, en modo consulta, la versión actual de Artículos y la última revisada por la tienda. Esta comparación permite ver el grado de actualización que tienen las ventas en relación a posibles cambios realizados.
*   En modo edición, es posible forzar el envío de todos los artículos existentes en la central a través del icono. Tras esta operación, se debe iniciar el proceso de sincronización para enviar todos los artículos a la tienda.

*   **Pestaña Tarifas**

En este apartado se insertarán todas las tarifas que se utilicen en la tienda.

Siempre existirá la tarifa GENERAL donde estarán todos los artículos.

Al igual que para la versión de artículos, se podrá forzar el envío de los datos de la tarifa en la próxima sincronización a través del icono .

*   **Pestaña Configuración**

Esta pestaña solo tendrá datos en el caso de que la tienda sea del tipo OFF-LINE Centralizada. En este apartado se identificarán los datos a través de los cuales el Sincronizador de la Central se conectará con la tienda. El campo Parámetros indica un conjunto de parámetros que permite una configuración adicional en la conexión con la base de datos de la tienda. En el caso de tratarse de MySQL, por defecto se indican los parámetros mostrados en esta pantalla, que configuran un timeout de conexión de 30 segundos.

Es posible consultar el archivo xml asociado a esta configuración pulsando sobre el botón “Ver XML”.

*   **Pestaña Usuarios**

En este apartado se insertarán todos los usuarios definidos para la Tienda. Todos ellos podrán interactuar con la Tienda.

*   **Pestaña Cajas**

Desde esta pestaña se podrán gestionar las distintas cajas pertenecientes a la tienda. También existe la posibilidad de descargar el fichero de configuración de cada caja desde la acción .

La acción permitirá descargar el archivo de instalación del POS completo.

La acción permitirá forzar la actualización de tarifa en la caja seleccionada.

Cuando se esté editando una tienda, tendremos la posibilidad de desactivar (), activar (), eliminar () o dar de alta una nueva caja (), según se aprecia en la siguiente imagen:

Para dar de alta nuevas cajas, se deben seleccionar aquellas cajas que estén disponibles del listado de cajas:

Tras aceptar la operación, las cajas seleccionadas estarán asociadas a la tienda.

#### Asistente de Alta de Tiendas {#asistente-de-alta-de-tiendas}

Mediante el botón Añadir existe la posibilidad de dar de alta tiendas a través de un asistente en el que se rellenarán los datos obligatorios de la tienda.

1.  Introducción de los datos generales de la Tienda:
2.  Introducción del tipo de tratamiento de impuestos asociado a la Tienda:
3.  Introducción de la tarifa asociada a la Tienda:
4.  Selección del Tipo de Sincronización de la Tienda con la Central:

*   En el caso de tipo de tienda **“OFF-LINE con Sincronización Centralizada”** requiere del detalle de parámetros de configuración:
*   El resto de casos de tipos de tienda no requieren parámetros de configuración:

1.  Selección de los usuarios asociados a la Tienda:
2.  Selección de las cajas asociadas a la Tienda:
3.  Finalización del proceso de alta de una Tienda:

### Mantenimiento de Conceptos de Almacenes Regularización {#mantenimiento-de-conceptos-de-almacenes-regularizaci-n}

Permite definir diferentes conceptos o motivos por los que sea necesario realizar una Regularización de almacén.

En este punto de menú se darán de alta los conceptos o motivos que se quieran contemplar en las Regularizaciones de almacén, de forma que, posteriormente, al dar de alta una Regularización de almacén, uno de los campos que se establecerá será el concepto por el que se realiza la Regularización.

Los campos de la pantalla son los siguientes:

*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: Nombre del concepto.
*   Signo: si permite sólo signos positivos, sólo negativos o ambos (en este caso, el campo estará en blanco)
*   Almacén de destino: se puede establecer el almacén de destino mediante la ayuda correspondiente.
*   Visible Tiendas: si se quiere que el concepto se pueda utilizar en las Tiendas.
*   Activo: si se puede utilizar.

Desde la pantalla de entrada a esta opción de menú se pueden listar todos los almacenes utilizando el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código y Descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Regularización:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

### Mantenimiento de Conceptos de Almacenes para Ventas {#mantenimiento-de-conceptos-de-almacenes-para-ventas}

La posibilidad de automatizar determinados criterios que se produzcan al realizar un pedido de Ventas.

En este punto de menú se darán de alta los conceptos que se quieran contemplar posteriormente en los procesos de ventas. Por ejemplo: Venta Directa, Venta a Tiendas, Devoluciones, etc.

Los campos de la pantalla son los siguientes:

*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: Nombre del concepto.
*   Signo: Se permitirá seleccionar entre (+)Positivo, (-)Negativo o ()Sin Signo.
*   Operación almacén: Vendrá condicionado por el signo seleccionado, tomando los valores: Entrada, Salida o No aplica.
*   Almacén Origen: para predeterminar el almacén de origen a través de la ayuda correspondiente.
*   Almacén destino: para predeterminar el almacén de destino recurriendo a la ayuda de almacenes.
*   Aceptación Automática de Pedidos: si se chequea esta casilla el Pedido de Venta no contemplará el estado PENDIENTE DE ACEPTACIÓN. De forma que pasará directamente del estado SOLICITUD DE PEDIDO al estado EN PREPARACIÓN.
*   Generación Automática de Pedido de Faltas: si se chequea esta casilla, para Pedidos de Venta, en el caso de que la cantidad pedida y la cantidad servida sean diferentes se generará automáticamente un pedido de faltas con la diferencia.
*   Visible en Tiendas: que el concepto sea visible en las tiendas.
*   Activo. si está en uso u obsoleto.

Desde la pantalla de Mantenimiento de Conceptos de Almacén para Venta se podrán listar todos los conceptos pulsando el botón **“Consultar”.**

También será posible filtrar por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Concepto de Almacén para Venta:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

### Mantenimiento de Conceptos de Almacenes para Compras {#mantenimiento-de-conceptos-de-almacenes-para-compras}

La posibilidad de automatizar determinados criterios que se produzcan al realizar un pedido de Compras.

En este punto de menú se darán de alta tantos conceptos como situaciones diferentes se produzcan en una operación de compras.

Los campos de la pantalla son los siguientes:

*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: nombre del concepto.
*   Signo: Se permitirá seleccionar entre (+)Positivo, (-)Negativo o ()Sin Signo.
*   Operación almacén: Vendrá condicionado por el signo seleccionado, tomando los valores: Entrada, Salida o No aplica.
*   Almacén destino: para predeterminar el almacén de destino.
*   Activo: si está en uso u obsoleto.
*   Aceptación Automática de Pedidos: si se chequea esta casilla el Pedido de Compra no contemplará el estado PENDIENTE DE ACEPTACIÓN. De forma que pasará directamente del estado SOLICITUD DE PEDIDO al estado EN PREPARACIÓN.
*   Generación Automática de Pedidos de Faltas: si se chequea esta casilla, para Pedidos de Compras, en el caso de que la cantidad pedida y la cantidad servida sean diferentes se generará automáticamente un pedido de faltas con la diferencia.

Desde la pantalla de Mantenimiento de Conceptos de Almacén para Compras se podrán listar todos los conceptos pulsando el botón “**Consultar”.**

También será posible filtrar por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Concepto de Almacén para Compras:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .