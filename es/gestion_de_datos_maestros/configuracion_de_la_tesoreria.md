## Configuración de la Tesorería {#configuraci-n-de-la-tesorer-a}

### Mantenimiento de Bancos {#mantenimiento-de-bancos}

Desde esta opción de menú se darán de alta los bancos con los que trabaja la empresa, así como los códigos de estos bancos.

Aunque es recomendable rellenar todos los campos porque de este modo se recuperarán automáticamente en otros procesos de la aplicación, los únicos campos obligatorios son el código, la descripción y los días de fin de riesgo remesados.

El significado de los campos de la pantalla es el siguiente:

*   Código: puede ser hasta de 11 dígitos
*   Descripción: Nombre del Banco
*   Domicilio: Calle, número, oficina.
*   Población
*   Provincia
*   Teléfonos
*   Fax
*   CCC: El CCC se dará de alta seguido, sin espacios ni guiones ni barras, ejemplo: 20980360150002005529.
*   CIF
*   CP
*   Observaciones: campo texto para insertar cualquier anotación a tener en cuenta.

Desde la pantalla de entrada a esta opción de menú se podrán listar todos los bancos pulsando el botón **Consultar.** Podrá filtrarse por código, descripción y registros activos.

Se listarán todos los bancos mostrando el código y la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Banco:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

Haciendo click sobre la opción **“Imprimir**”, se llega a la siguiente pantalla en la que se muestran las distintas versiones del informe de listado de bancos:

### Mantenimiento de Tipos de Efectos {#mantenimiento-de-tipos-de-efectos}

Los tipos de efecto permiten agrupar los diferentes Medios de Pago y definir cuáles de ellos van a ser al contado.

En este punto de menú se definirán los diferentes Tipos de Efecto que se vayan a utilizar, por ejemplo: Pagaré, Giro, Contado, Transferencia, etc. Posteriormente, en el Mantenimiento de Medios de Pago se asociará a cada forma de pago el Tipo de efecto que le corresponda.

Los campos de la entidad Tipo de Efecto son los siguientes:

*   Código: puede ser alfanumérico de 2 dígitos.
*   Descripción: Nombre del Tipo de Efecto.
*   Remesable: si se gestiona a través de Remesas al banco.
*   Entrada Documento Automática: indica si es de Aceptación Automática, es decir, que no es necesaria la validación del cliente para el envío del documento al banco. Por ejemplo, esto ocurre con los Giros.
*   Activo: indica si el registro está activo u obsoleto.

Desde la pantalla de entrada a esta opción de menú se podrán listar todos los tipos de efectos pulsando el botón “**Consultar”.** Podrá filtrarse por código, descripción y registros activos.

Los Resultados mostrarán el código y la descripción de cada registro.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Tipo de Efecto:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .

### Mantenimiento de Medios de Pago {#mantenimiento-de-medios-de-pago}

En este punto de menú se definirán las formas de pago disponibles en la aplicación para que puedan utilizarse en los procesos de ventas y compras. Está ubicado dentro del menú **“Común”.**

El Mantenimiento de los Medios de Pago es muy importante para la gestión correcta de la Tesorería, ya que en función de la definición de éste Mantenimiento se generarán los vencimientos.

La pantalla tiene dos bloques:

En el primer bloque se identifican los **“Datos del Medio de Pago”:**

*   Código: puede ser alfanumérico de hasta 4 dígitos.
*   Descripción: Nombre del medio de pago.
*   Activo: si está en uso.
*   Recuento automático Caja.

En el segundo Bloque aparecen una o dos pestañas dependiendo de la forma de pago. En el caso de que la forma de pago sea al contado (esté chequeada la casilla “Contado”), no aparece la pestaña de **“Vencimientos”.** Si la casilla “Contado” no está chequeada sí aparece la pestaña de Vencimientos para indicarlos.

El significado de los campos es el siguiente:

1.  **Pestaña Datos Generales:** en el apartado Modalidad habrá que indicar si la forma de pago es Contado o no, si se chequea la casilla “contado” aparecerán dos campos para indicar el tipo de contado: Efectivo o Tarjeta de Crédito:

El campo Tipo de efecto será un campo de tipo ayuda que recuperará los Tipos de efectos dados de alta en el Mantenimiento de Tipos de Efecto (punto 4.3.2 de este manual). Los tipos de efecto servirán para agrupar los medios de pago, de forma que, por ejemplo, podrán existir los medios de pago: Pagaré a 30 días, Pagaré a 60 días, Pagaré a 90 días; y todos ellos tendrán asociado el Tipo de efecto Pagaré.

En el apartado Visibilidad se indica si el medio de pago es visible en los procesos de compras, ventas y en la tienda virtual. La casilla &quot;Manual&quot; permite al usuario indicar si ese medio de pago se aplicará de forma manual en los procesos de venta.

La casilla de Tienda Virtual sólo aparece en los medios de pago de contado, es decir, que esté chequeada la casilla **“Contado”.**

1.  **Pestaña Vencimientos:**

Cuando la forma de pago no es contado, es necesario identificar los vencimientos. Para insertar o modificar un vencimiento, hay que editar primero (icono de la cabecera) y se activará en el detalle el icono para crear un nuevo vencimiento.

En el vencimiento se debe indicar:

*   Descripción: descripción general del vencimiento, por ejemplo “pagare 30, 60”
*   Nº de vencimientos: número de vencimientos que tendrá la modalidad de pago
*   Días de cadencia: número de días hasta el primer vencimiento
*   Días entre vencimientos: número de días entre vencimientos
*   Naturales: identifica si los días anteriores serán naturales o no.

**Ejemplo: Pagaré 30, 60**

*   Nº de vencimientos: 2
*   Días Cadencia: 30
*   Días entre vencimientos: 30

Desde la pantalla de entrada de esta opción de menú se podrán listar todas las formas de pago mediante el icono **“Consultar”.**

Se pueden establecer criterios de búsqueda opcionales utilizando los campos del código y descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Medio de Pago:

*   Para dar de alta un registro hay que posicionarse sobre el botón Añadir de la cabecera.
*   Para Editar un registro se utilizará el icono de la barra de acciones.
*   Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono
*   Para dar de baja un registro se utilizará el icono .