# INTRODUCCIÓN

## Acerca de este manual

Este manual proporciona una Guía para el Usuario del BACKOFFICE del sistema comerzzia detallándose las funcionalidades de la aplicación. Los lectores no requieren ningún conocimiento acerca de programación ni desarrollo de software.

## Qué hay de nuevo en el manual de usuario 4.0

  - Reestructuración de menús.

  - Configuración de Tipos de Servicios, Calendarios de servicios y Consulta de servicios.

  - Nuevo punto de menú para Importación masiva de etiquetas.

  - Nuevos mantenimientos asociados a preparaciones y Artículos: Mantenimiento de Unidades de Medida, Preferencias de sustitución en pedidos, Tipos de Embalaje.

  - Incorporación de mejoras en el Mantenimiento de Tiendas y configuración de servicios asociados.

  - Mejoras en la Gestión de solicitudes y mantenimientos asociados.

## Documentación relacionada

  - Guía de Navegación comerzzia

  - COM\_ADM\_GUÍA DE IMPLANTACIÓN, PARAMETRIZACIÓN Y PERSONALIZACIÓN

  - COM\_INS\_MANUAL DE INSTALACIÓN EN TIENDA

  - COM\_USR\_MANUAL DEL POS JAVA

# CONFIGURACIÓN GENERAL

## Asistente de Configuración de Empresa

El backoffice de comerzzia dispone de un Asistente de Configuración de la Empresa, que se ejecuta de forma automática en caso de detectar que tal configuración no está implementada en el sistema. Para configurar una empresa se sigue un proceso secuencial que facilita el registro de una empresa paso a paso.

1)  Selección del tipo de parametrización de la empresa que se va a dar de alta:

<!-- end list -->

  - **Multiempresa:** Configuración destinada a empresas que, por su volumen de facturación, esté conformada por un conjunto de sociedades. Bajo esta configuración se parametrizarán el conjunto de empresas y todas compartirán los mismos datos de clientes, artículos y datos de tablas maestras.

  - **Multiactividad:** Configuración destinada a empresas que, debido a que sus actividades están enfocadas en diferentes áreas (ejemplo, fabricación, distribución. etc...) crean sociedades diferentes para cada propósito. En este caso, se parametrizarán el conjunto de empresas pero no compartirán los mismos datos de clientes, artículos y datos de tablas maestras.

![](/media/image2.png)

2)  Datos de la empresa: Los datos de la empresa a registrar en comerzzia son:
    
      - Código: Código identificativo de la empresa de 4 dígitos numéricos.
    
      - Descripción: Nombre de la empresa.
    
      - Domicilio: Domicilio fiscal de la empresa.
    
      - Población: Localidad.
    
      - Provincia: Provincia.
    
      - CP: Código Postal.
    
      - CIF: Código de Identificación Fiscal de la empresa.
    
      - Teléfono 1: Teléfono de contacto.
    
      - Teléfono 2: Teléfono de contacto alternativo.
    
      - Fax: Número de fax.
    
      - Registro Mercantil.

![](/media/image3.png)

3)  Selección de logo de la empresa. Se permite subir una imagen y que quede establecida como logotipo de la empresa.

![](/media/image4.png)

Datos del almacén central: Para toda empresa que se registra se debe establecer una central. Por defecto al almacén central se le asigna el código y el país de registro de la empresa, y la descripción “ALMACÉN CENTRAL”. Además existe un check para marcar si el almacén central es además una tienda.

  - Código: Código identificativo de 4 dígitos numéricos.

  - Descripción: Nombre del Almacén.

  - Domicilio, Población, Provincia, Código Postal: correspondientes a la ubicación física del almacén.

  - Teléfonos y Fax.

  - Persona de Contacto.

Si se marca el Almacén como “Este Almacén es una Tienda”, el asistente dará de alta la **TIENDA** del tipo “ON-LINE” con el mismo código que el almacén central.

![](/media/image5.png)

4)  Datos del cliente: Se registra un cliente por defecto al que se le asignarán las ventas.

![](/media/image6.png)

## Configuración de la Empresa

En esta opción de menú podemos especificar los datos generales de nuestra empresa, así como la imagen (logo) corporativa.

![](/media/image7.png)

Los datos de la empresa registrados en comerzzia son:

  - Código: Código identificativo de la empresa. 4 dígitos numéricos (0000)

  - Descripción: Nombre de la empresa

  - Domicilio: Domicilio fiscal de la empresa

  - Población: Localidad

  - Provincia: Provincia

  - CP: Código Postal

  - CIF: CIF de la empresa

  - Teléfono 1: Teléfono de contacto

  - Teléfono 2: Teléfono de contacto alternativo

  - Fax: Número de fax

  - Registro Mercantil.

### Cambiar Logotipo

Tenemos la posibilidad, desde esta pantalla, de cambiar el logo corporativo

![](/media/image8.png)

![](/media/image9.png)

## Configuración de los parámetros del Sistema

Se trata de una pantalla de Administración de variables internas del sistema, que nos permitirá definir una configuración personalizada para nuestro sistema:

![](/media/image10.png)

A continuación se detallan las variables configurables en el sistema:

### Variables configurables: Artículos

![](/media/image11.png)

  - “Título para el primer desglose en almacén”.

  - “Título para el segundo desglose en almacén”.

  - "Formato de los códigos de barras aleatorios".

Los dos “niveles de desglose” son opcionales (Talla y Color para el ejemplo representado) y, en caso de decidir usarlos, son los nombres que dinámicamente recogerán las pantallas del sistema.

El formato de los códigos de barras aleatorios puede ser EAN13 o EAN18 (este último es el valor por defecto); los códigos de barras generados de forma aleatoria en el mantenimiento de artículos tendrán un formato u otro según la opción seleccionada.

![](/media/image12.png)

### Variables configurables: Tarifas

![](/media/image13.png)

  - Primer nivel de redondeo de tarifas. Desde/Hasta/Valor

  - Segundo nivel de redondeo de tarifas. Desde/Hasta/Valor

  - Tercer nivel de redondeo de tarifas. Desde/Hasta/Valor

Con estos parámetros se establece una **forma opcional de hacer redondeo**, sobre las dos primeras posiciones decimales de los precios (PVP+impuestos) en tarifa, en el proceso de “Actualización masiva de Artículos en la Tarifa”, descrito en apartado posterior de este manual, específico de proceso de Ventas y gestión de Tarifas.

Como podemos observar se establecen rango de valores desde/hasta y valor asignado para la posición decimal correspondiente.

### Variables configurables: TPV

![](/media/image14.png)

  - “Uso de descuentos en líneas para los tickets realizados por el POS”: es posible activar esta posibilidad de aplicar descuento a nivel de línea de detalle en los documentos de venta.

  - “Realizar la venta de artículos con precio 0”: posibilidad de activar o desactivar la opción que permite vender artículos con precio 0.

  - “Permitir el cambio de precio en edición”: posibilidad de modificar el precio de los artículos desde la pantalla de edición de línea.

  - “Para finalizar una venta la fecha de apertura de caja deberá ser igual a la fecha del sistema: Permite incorporar un control más en el proceso de venta para no poder hacer ventas en día diferente al de apertura de la caja. En el caso de que exista un ticket aparcado o una venta en curso, sí se permitirá acceder a la pantalla de ventas.

  - “Realizar apertura automática de caja al entrar en las pantallas de venta”: Permite configurar la apertura automática de la caja al iniciar con el proceso de venta.

  - “Columna vendedor visible en la pantalla de ventas del POS”: Permite visualizar el vendedor asociado a cada línea de la pantalla de Ventas del POS.

  - “Aplicar promociones de precio antes que el resto, que se aplicarían sobre el precio promoción”: Permite configurar las promociones de forma que las promociones de precio de artículos se apliquen antes que el resto de promociones activas, aplicándolas a posteriori sobre el precio fijado en la promoción de precio y no sobre el de tarifa. Además, si se marca este campo, los artículos que tengan promociones de tipo “Precio/Puntos” se mostrarán en la tienda virtual con el precio sin promoción tachado, junto al precio con descuento.

  - "Número de reintentos para cerrar la caja con descuadres": Indicamos el número máximo de intentos que se permiten para poder cerrar la caja con descuadres.

  - “Tener en cuenta en las devoluciones las promociones menos ingreso del ticket origen”: Considerar, al hacer una devolución, el precio con promoción existente en el momento en que se hizo la compra.

### Variables configurables: Servicios REST 

![](/media/image14.png)

Indica la clave de acceso a los servicios REST de comerzzia.

## Mantenimiento de Sitios

En comerzzia el concepto de sitio hace referencia a la configuración de un entorno, donde se definen las variables y opciones de configuración de una tienda virtual. Se incluye por tanto un mantenimiento de sitios que permite la gestión de dichas configuraciones. Este mantenimiento se encuentra en el menú **Sistemas -\> Empresa.**

Para consultar el listado de sitios disponibles se emplea un buscador que puede filtrar por código y por descripción.

![](/media/image15.png)

Desde esta pantalla se permiten las siguientes funcionalidades:

  - Para dar de alta un nuevo sitio hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un sitio se utilizará el icono![](/media/image19.png).

Para la definición de un sitio, deben rellenarse los campos:

![](/media/image20.png)

  - **Código:** valor alfanumérico único para cada sitio.

  - **Descripción:** título identificativo del sitio.

  - **URL base:** URL base a la que hace referencia la configuración del sitio. La URL introducida debe incluir el prefijo para que sea válida.

Adicionalmente un sitio requiere de una conjunto de configuración adicional, para asegurar el correcto funcionamiento del mismo:

**<span class="underline">Datos Generales:</span>** Desde esta pestaña se definen:

![](/media/image21.png)

*Opciones de configuración de la tienda:*

  - **Tienda:** Código y descripción de la tienda asociada al sitio. Esta tienda será la que defina tanto la empresa como el canal de venta y medios de pago que le corresponden.

  - **Modo de tienda:** Combo que permite definir el modo de funcionamiento asociado a la Tienda Virtual, siendo:
    
      - Modo clásico: La tienda virtual muestra en los portlets de escaparate y detalle de artículo sólo los artículos configurados para el canal de venta de la tienda virtual.
    
      - Modo avanzado: La tienda virtual muestra en los portlets de escaparate los productos configurados para el canal de venta de la tienda virtual, y, en el detalle de cada producto, la información del producto consultado y de los artículos asociados, si dicho producto tiene configurado más de un artículo. Estos artículos son los que se podrán comprar, no el producto en sí mismo.  
        El comportamiento a nivel de promociones en este modo será el siguiente:

<!-- end list -->

  - Si un producto solo tiene 1 artículo con o sin desgloses, y dicho artículo tiene promociones, el producto mostrará el icono asociado a dicha promoción tanto en el portlet de listados de productos (escaparate, productos relacionados), como en el de detalle de producto/artículo.

  - Si un producto tiene más de 1 artículo con o sin desgloses, y dichos artículos tienen promociones, el producto mostrará un icono genérico de promoción en el portlet de listados de productos (escaparate, productos relacionados). En el detalle de producto/artículo se mostrará la promoción específica de cada artículo asociado al producto.

> En cuanto a las características de producto, se mostrarán a nivel del producto las asociadas a las etiquetas del producto, y, para cada artículo del producto las asociadas a sus etiquetas.

*Opciones de configuración de artículos:*

![](/media/image22.png)

  - **Mostrar artículos sin disponibilidad:** Casilla que se marca si se desea que en los listados de productos de la tienda virtual se muestran aquellos cuya disponibilidad en la propia tienda sea inferior a una cantidad.

  - **Mostrar filtro de disponibilidad de artículos.** En el caso de tener activo el check 'Mostrar artículos sin disponibilidad', muestra un filtro para que se muestren sólo aquellos que están disponibles.

  - **Permitir comprar sin disponibilidad de artículos.** Si existen productos que no están disponibles, permite añadirlos a la cesta. Tiene que estar activo el check 'Mostrar artículos sin disponibilidad'.

*Opciones de configuración de Informes:*

![](/media/image23.png)

1)  **Ruta base de informes:** URL asociada a la ubicación de los informes asociados al sitio.

*Opciones de configuración de Imágenes:*

A partir de esta versión 4.0.4 es necesario configurar las rutas de las imágenes multimedia utilizadas en la Tienda Virtual, APP y FastPOS. **”. **

En función de los módulos contratados por cada cliente y SECTOR, será necesario configurar el conjunto de URLs que a continuación se detallan.

![app-alert-icon](/media/image24.png) En caso de no llevar a cabo esta configuración, las imágenes no se cargarán.

![](/media/image25.png)

Siendo:

  - **FOOD/NON-FOOD Tienda Virtual/APP/FASTPOS: **
    
      - **Ruta imágenes artículos:** Imágenes asociadas a los artículos mostradas en los portlets de listados de artículos y detalle de artículos.
    
      - **Ruta imágenes productos:** Imágenes asociados a los productos en configuración de tienda avanzada (Producto principal que engloba a N artículos, principalmente sector Perfumerías).
    
      - **Ruta imágenes promociones:** Imágenes asociadas a las promociones posibles de aplicar en cada artículo, mostradas al visualizar el listado de artículos y el detalle.
    
      - **Ruta imágenes características:** Imágenes asociadas a las características concretas asociadas a cada artículo.
    
      - **URL detalle producto:** URL asociada a la página de detalle de un producto.

  - **Sólo FOOD Tienda Virtual: **
    
      - **Ruta imágenes categorías:** Imágenes asociadas al menú superior de categorías. Son opcionales, en función de la configuración de dicho menú.
    
      - **Ruta imágenes categorizaciones:** Imágenes asociadas al portlet de submenú de categorías incluido de forma opcional dentro de la página de una categoría concreta.

  - **Sólo NON-FOOD APP e-commerce: **
    
      - **Ruta imágenes desgloses:** Imágenes asociadas a los selectores de desgloses incluidos en la página de detalle de artículo. En la tienda virtual no se utiliza al mostrarse esta información en modo texto.

  - **Sólo NON-FOOD APP e-commerce/FASTPOS: **
    
      - **Ruta imágenes menú:** Imágenes asociadas a la HOME.

**<span class="underline">Configuración adicional:</span>** Desde esta pestaña se definen:

![](/media/image26.png)

  - **Ruta de BrainSINS:** Referencia al archivo que contiene el catálogo de artículos al que accede el recomendador de BrainSINS.

  - **Token:** Token para la comunicación con BrainSINS.

  - **Imagen de error:** URL que dirige a la imagen establecida como error para referir a artículos que no tengan imagen asociada en Liferay.

Además, se dispone de la opción de **“Generar XML feed”** mediante la que se genera de forma manual la información de artículos que requiere “Brainsins” para poder realizar recomendaciones de productos.

![](/media/image1.png)Esta operación es necesaria lanzarla al menos la primera vez que se active el recomendador de productos Brainsins.

Además, será necesario actualizar el catálogo al que accede BrainSINS cada vez que se modifique el surtido disponible o se suban nuevas imágenes de artículos al portal de Liferay, etc…para que disponga de toda la información de la tienda actualizada.

**<span class="underline">Servicios</span>**

Desde esta pestaña se muestran los diferentes tipos de servicios que se ofrecen desde el sitio. Desde el modo edición, se permiten añadir o eliminar nuevos tipos de servicio, además de establecer el tipo de servicio por defecto.

![](/media/image27.png)

**<span class="underline">XML</span>**

Toda la información de configuración asociada al sitio consultado es posible visualizarla en formato XML a través de esta interfaz.

## Configuración de Ayudas

Se trata de una opción de configuración existente, pero **no administrable por el usuario final**, sino orientada al usuario encargado de desarrollo de backoffice.

La pantalla principal de esta opción de menú muestra el listado de ayudas existentes así como el campo de búsqueda nombre.

![](/media/image28.png)

Permite establecer los datos a representar y los criterios de búsqueda en las pantallas tipo AYUDA. Las Ayudas son un recurso auxiliar del sistema que permiten listar y seleccionar elementos de tablas maestras, necesarios para la gestión de otras entidades, documentos o procesos.

![](/media/image29.png)

## Configuración de Menús

La configuración de menús será **parametrizable**, pero dicha posibilidad **no será accesible al usuario final**. Esto se hace desde una aplicación de escritorio adicional al backoffice de comerzzia. El sistema sí dispondrá de cuatro configuraciones (lo que en comerzzia se denomina APLICACIÓN) precargadas (ADMINISTRACIÓN, SISTEMA, CENTRAL, INVOLVECRM y BACKOFFICE) que a continuación mostramos:

![](/media/image30.png)![](/media/image31.png)![](/media/image32.png)

![](/media/image33.png)![](/media/image34.png)

Tal como se describe en apartado posterior de MANTENIMIENTO DE USUARIOS, a cada usuario se le puede asociar un APLICACIÓN por defecto y la posibilidad o no de cambiar de Menú.

# SEGURIDAD - PERMISOS

## Mantenimiento de Perfiles ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\perfiles.gif](/media/image35.gif)

Permite listar los Perfiles de Usuario, así como dar altas, editar y consultar los perfiles existentes.

En la pantalla de entrada a esta opción de menú, se ofrece la posibilidad de **listar los Perfiles**, mostrando tabla de resultados con la siguiente información:

![](/media/image36.png)

Se pueden establecer **criterios de búsqueda** opcionales en base a los siguientes conceptos:

  - Descripción del Perfil

A través de esta **pantalla** tenemos la posibilidad de **navegar hacia otras páginas** que me permitirán:

  - Dar el alta un nuevo Perfil ![](/media/image37.png)

  - Consultar y editar los datos de un Perfil existente ![](/media/image38.png)

  - Eliminar Perfiles ![](/media/image39.png)

Para Dar de alta un perfil, será necesario especificar el campo “Descripción” asociado al perfil.

![](/media/image40.png)

## Mantenimiento de Usuarios ![](/media/image41.png)

Permite listar los Usuarios del sistema, así como dar altas, editar y consultar los Usuarios existentes. A través de este Mantenimiento el sistema ofrece la posibilidad de cambiar las contraseñas (password) de acceso a la aplicación.

### Listado de Usuarios

Es la pantalla de entrada a esta opción de MENÚ. Ofrece la posibilidad de **listar los Usuarios**, mostrando tabla de resultados con la siguiente información:

![](/media/image42.png)

Se pueden establecer **criterios de búsqueda** opcionales en base a los siguientes conceptos:

  - Código del Usuario

  - Descripción del Usuario

  - Todos/Activos/Inactivos

A través de esta **pantalla** tenemos la posibilidad de **navegar hacia otras** que me permitirán:

  - Dar el alta un nuevo Usuario ![](/media/image37.png)

  - Consultar y editar los datos de un Usuario existente ![](/media/image38.png)

  - Eliminar Usuarios ![](/media/image39.png)

### Atributos de Usuario

Un Usuario en comerzzia se define de la siguiente manera:

  - DATOS DEL USUARIO:

![](/media/image43.png)

  - Usuario: Código del Usuario.

  - Descripción: Nombre descriptivo del usuario.

  - Menú por defecto: referencia a ayuda de Menú (configuración/agrupador de menús). Si se especifica será el menú mostrado por defecto cuando el usuario se logue en el sistema.

  - Activo: Usuario en uso para el sistema.

  - Puede cambiar de aplicación (Sí/No): respecto a la que se le ha especificado por defecto.

  - Contraseña: Contraseña de acceso al sistema.

  - Confirmar Contraseña: Confirmación de contraseña introducida anteriormente.

<!-- end list -->

  - DETALLE DE PERFILES:

![](/media/image44.png)

  - Perfil: referencia del maestro de Perfiles

> El botón ![](/media/image45.png) permite asignar un perfil al usuario en cuestión.

  - DETALLE DE ALMACENES: en los que el usuario tendrá acceso

![](/media/image46.png)

  - Almacén: Referencia del maestro de Almacenes

El botón ![](/media/image47.png) permite asignar un almacén al usuario en cuestión.

### Alta / Edición / Consulta de un Usuario

A través de pantallas específicas (navegación desde el Listado de Usuarios) se accede al mantenimiento de los datos de un Usuario (altas / ediciones / consultas).

  - ![](/media/image16.png) Añadir: Permite dar de alta un nuevo Usuario

  - ![](/media/image38.png) Consultar / Editar: Permite Consultar y/o Editar el Usuario.

La enumeración y descripción de campos que constituyen un Usuario se ha hecho en el apartado anterior de “Atributos de Usuario”.

### Restablecer contraseña

Desde esta pantalla de Administración el sistema ofrece la posibilidad de cambiar la password de los Usuarios.

Se accede a la citada funcionalidad a través de menú contextual de acciones RESTABLECER CONTRASEÑA:

![](/media/image48.emf)

Navegando a pantalla donde nos pedirá por duplicado que informemos sobre la nueva clave de acceso.

![](/media/image49.png)

Un usuario sin acceso al Mantenimiento de Usuarios podrá restablecer su propia contraseña a través de la página “MI PERFIL”, descrita en apartado anterior de este manual.

### Baja de un Usuario

![](/media/image50.png) Eliminar Permite Eliminar un Usuario

## Configuración de Permisos

Sobre cada una de las pantallas existen opciones (menú contextual de acciones) que nos permiten consultar y administrar los permisos.

![](/media/image51.png)

### Consultar Mis Permisos

Con la opción ![](/media/image52.png) desde cada pantalla del sistema puedo consultar mis privilegios sobre la misma:

![](/media/image53.png)

Donde, sobre cada una de las opciones (EJECUTAR / AÑADIR / EDITAR / ELIMINAR), obtenemos información en base a la siguiente nomenclatura:

![](/media/image54.png) OPCIÓN ADMINISTRABLE, es decir, el usuario o perfil sobre el que se informa puede gestionar los derechos de otros usuarios sobre la opción seleccionada

![](/media/image55.png) Indica que el usuario o perfil sobre el que se informa TIENE DERECHOS sobre la opción

![](/media/image56.png) Indica que el usuario o perfil sobre el que se informa NO TIENE DERECHCOS sobre la opción

### Administrar Permisos

Con la opción ![](/media/image57.png) desde cada pantalla del sistema puedo, si tengo privilegios, administrar los permisos sobre cada una de las opciones de esa pantalla, a nivel de perfiles y de usuarios particulares

![](/media/image58.png)

Sobre esta pantalla se pueden añadir usuarios y perfiles, mediante las opciones ![](/media/image59.png) y![](/media/image60.png). Asimismo se podrá modificar sus permisos al hacer click sobre cada uno de los iconos “semáforo” de esta matriz.

# GESTIÓN DE DATOS MAESTROS

Este apartado enumera y describe las entidades básicas que han de definirse y configurarse en la aplicación, como soporte a los procesos de negocio que el sistema comerzzia da servicio.

## General

### Mantenimiento de Series ![](/media/image61.gif)

El concepto de Serie se identifica con las diferentes delegaciones o zonas geográficas. Deberá existir al menos una serie con el código 0000 para asociar a los documentos.

![](/media/image62.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de 5 dígitos.

  - Descripción: Nombre identificativo de la serie

  - Activo: identifica si el registro está en uso u obsoleto.

La serie se identifica como un criterio para agrupar los diferentes documentos que se van a generar en la aplicación, por ejemplo: albaranes, facturas, etc.

La pantalla de entrada a esta opción de MENÚ ofrece la posibilidad de listar las diferentes Series que se hayan dado de alta, mostrando la tabla de resultados con la siguiente información:

![](/media/image63.png)

Se pueden establecer búsquedas por código o descripción; en caso contrario, al consultar, se listarán todas las Series que existan.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una serie.

  - Para dar de alta una Serie hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Países ![](/media/image64.png)

En este punto de menú se darán de alta los Países para posteriormente utilizarlos en otras pantallas de la aplicación. Por ejemplo, en el Mantenimiento de Clientes y Proveedores. Es conveniente codificar los países en base a los códigos que maneja el Instituto de Estadística: alfabético de 2 o 3 dígitos; por ejemplo: España: ES.

![](/media/image65.png)

Por defecto en comerzzia están precargados todos los países.

![](/media/image66.png)

Los campos de la pantalla son los siguientes:

  - Código: Código asociado al país de tipo alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre identificativo del País

  - Activo: identifica si el registro está en uso u obsoleto.

La pantalla de entrada a esta opción de MENÚ ofrece la posibilidad de listar los diferentes Países que se hayan dado de alta, mostrando la tabla de resultados con la información anterior.

Se pueden establecer búsquedas por código, descripción y estado activo o no. En caso de no introducir nada, al consultar, se listarán todos los Países que existan.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una País.

  - Para dar de alta una País hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Códigos Postales ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\mantenimiento-codigopostal.gif](/media/image67.gif)

Asociado a cada País, Provincia y población se podrán dar de alta códigos postales.

![](/media/image68.png)

Los campos de la pantalla son los siguientes:

  - Código: Código asociado al código postal.

  - País: País asociado al código postal.

  - Población: Población asociada al código postal.

  - Localidad: Opcional, localidad asociada al código postal.

  - Provincia: Provincia asociada al código postal.

La pantalla de entrada a esta opción de MENÚ ofrece la posibilidad de listar los diferentes códigos postales que se hayan dado de alta, mostrando la tabla de resultados con la información anterior.

Se pueden establecer búsquedas por código postal, país, población, localidad y provincia. En caso de no introducir nada, al consultar, se listarán todos los códigos postales que existan.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Código Postal.

  - Para dar de alta un Código Postal hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Divisas![](/media/image69.gif)

Desde este mantenimiento será posible gestionar las diferentes Divisas con las que trabajará la plataforma de comerzzia en caso de ser necesario por la distribución geográfica de la Red de Tiendas.

![](/media/image70.png)

Los campos de la pantalla son los siguientes:

  - Código: Código asociado a la Divisa.

  - Descripción: Descripción asociada a la Divisa.

La pantalla de entrada a esta opción de MENÚ ofrece la posibilidad de listar las diferentes divisas que se hayan dado de alta, mostrando la tabla de resultados con la información anterior.

Se pueden establecer búsquedas por código y descripción. En caso de no introducir nada, al consultar, se listarán todas las divisas que existan.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Divisa.

  - Para dar de alta una Divisa hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Categorías de Etiquetas

A través de este mantenimiento el sistema permite gestionar las categorías de etiquetas, que serán de utilidad principalmente tanto en la tienda virtual como en la generación de promociones y el uso de acciones comerciales.

En este punto se dan de alta las Categorías de Etiquetas para, posteriormente, en el mantenimiento de artículos, categorizaciones y fidelizados tener la posibilidad de asociar a cada artículo/categorización una o varias etiquetas.

La búsqueda de categorías se hace por descripción. Las funcionalidades de este mantenimiento son:

  - Dar de alta una nueva categoría de etiquetas desde el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar una categoría mediante el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Eliminar una categoría de etiquetas utilizando el icono![](/media/image19.png).

![](/media/image71.png)

El único campo necesario es la descripción de la categoría. Además, se puede establecer de manera opcional una prioridad entre las diferentes categorías.

Tras acceder a una categoría concreta, será posible crear, asociar o eliminar etiquetas existentes, tras pulsar el botón **“Editar”:**

![](/media/image72.png)

NOTA: Toda etiqueta utilizada en comerzzia deberá estar asignada a una Categoría de Etiquetas para asegurar su funcionamiento en la Tienda Virtual, promociones y cualquier otro módulo que haga uso de las mismas.

### Mantenimiento de Etiquetas

Los artículos, categorizaciones y fidelizados en comerzzia pueden tener asociadas etiquetas que estarán englobadas dentro de una determinada categoría.

Desde el mantenimiento de etiquetas se permite la consulta de todas las etiquetas definidas y la categoría a la que corresponde. Una etiqueta puede pertenecer a más de una categoría, por lo que desde la tabla de consulta de etiquetas se muestran todas las relaciones de las etiquetas con una categoría. Para realizar esta consulta se puede filtrar por la descripción o por categorías.

Además, desde este mantenimiento se permite:

  - Dar de alta una etiqueta, pulsando sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Editar un registro se utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar una etiqueta en concreto haciendo ‘click’ sobre el icono![](/media/image18.png).

  - Eliminar una etiqueta utilizando el icono![](/media/image19.png).

![](/media/image73.png)

Para la definición de una etiqueta, el único campo obligatorio es la descripción. Sin embargo, también puede gestionarse desde la pantalla de detalle de una etiqueta su relación con las diferentes categorías. Esta relación se concreta con una prioridad en la categoría, que determina la prioridad de una etiqueta dentro de una categoría.

![](/media/image74.png)

### Funcionalidad de Importación masiva de etiquetas ![](/media/image75.png)

La versión 4 de comerzzia incluye una nueva funcionalidad realizar diferentes tipos de importaciones a comerzzia. Este punto de menú se encuentra en **“Administración-\>Común”**

![](/media/image76.png)

Los campos que definen la importación son:

  - Tipo de importación: Campo de tipo combo que permite seleccionar el tipo de importación que desea llevarse a cabo de entre las disponibles.

  - Ámbito de aplicación: Campo de lectura donde se muestra la aplicación que tiene el tipo de importación seleccionado en el combo.

  - Descargar plantilla de importación: Mediante este botón se descarga la plantilla Excel para la posterior importación de datos.

Las plantillas de importación deben ubicarse en la carpeta plantillas\_importacion, en la carpeta de recursos de comerzzia. El nombre de dichas plantillas será el formado por idaccion\_ejecucion de la acción correspondiente al tipo de importación.

  - Fichero: Se selecciona el archivo que desea importarse a comerzzia.

Una vez configurada la importación que se llevará a cabo, se selecciona el botón Importar.

Tras esto, se muestra una pantalla de resumen que muestra las posibles incidencias que se hayan ocasionado a partir del proceso de importación.

![](/media/image77.png)

### Mantenimiento de Tipos de Solicitudes ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\mantinimientoTipoSolicitudes.gif](/media/image78.gif)

El mantenimiento de tipos de solicitudes cuelga del menú **“Administración -\> Fidelización”** del backoffice de comerzzia. Desde aquí se pueden consultar las diferentes tipologías de las solicitudes que podrá hacer el cliente. Para realizar la búsqueda se puede filtrar por código y descripción de la solicitud, además de permitir búsqueda sólo de registros activos.

![](/media/image79.png)

Las funcionalidades del mantenimiento de tipos de solicitudes son:

  - Dar de alta un nuevo tipo de solicitud: Pulsando sobre ![](/media/image16.png) Añadir se procede a la creación de un nuevo tipo de solicitud. Los campos a cumplimentar son:

![](/media/image80.png)

  - Código: Unitario para cada tipo de solicitud, puede ser alfanumérico de 4 dígitos.

  - Descripción: Nombre del tipo de solicitud

  - Visible cliente: Se marca si el tipo de solicitud va a ser accesible para los clientes

  - Activo: Permite definir cuando un tipo de solicitud se va a encontrar activo/inactivo.

<!-- end list -->

  - Consultar un tipo de solicitud existente, pulsando sobre ![](/media/image17.png) en la tabla de resultados.

  - Editar la información de un tipo de solicitud. ![](/media/image18.png)

  - Eliminar un tipo de solicitud, haciendo click en ![](/media/image19.png)

## Configuración de Impuestos

La definición de los distintos impuestos se hace a través de tres mantenimientos de la aplicación, que se encuentran en el menú **“Sistema -\> Impuestos”:**

  - Mantenimiento de Tipos de Impuestos

  - Mantenimiento de Tratamiento de Impuestos

  - Mantenimiento de Cuadro de Impuestos

### Mantenimiento de Tipos de Impuestos ![](/media/image81.gif)

En este Mantenimiento se darán de alta los diferentes tipos impositivos que maneje la empresa, Por ejemplo: Normal, Reducido, Exento.

![](/media/image82.png)

Los datos que habrá que indicar serán el código y la descripción.

La pantalla de entrada a esta opción de MENÚ permite listar los diferentes tipos de impuestos que se hayan dado de alta, siendo posible filtrar por el código o la descripción.

![](/media/image83.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Tipo de Impuesto:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Tratamiento de Impuestos ![](/media/image84.png)

En este punto de menú se darán de alta los impuestos que se apliquen.

Por ejemplo: Nacional, Intracomunitario/Exportaciones, Nacional exento de IVA, Nacional con recargo de equivalencia, IGIC, IPSI, etc.

![](/media/image85.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 11 dígitos.

  - Descripción: Nombre identificativo del impuesto

  - País: País de aplicación asociado al impuesto.

  - Región de Impuestos: Región en la que se aplica el impuesto anterior.

  - Aplica recargo: chequear en los casos en los que se deba aplicar recargo de equivalencia

Desde la pantalla de entrada de esta opción de menú, pulsando el botón CONSULTAR se podrán listar todos los Tratamientos de Impuestos que se hayan dado de alta, pudiendo restringir por los campos de código o descripción.

![](/media/image86.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Tratamiento de Impuestos:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Cuadro de Impuestos ![](/media/image87.png)

En este punto de menú se asociará a cada Tratamiento de Impuesto un tipo de impuesto, identificando la vigencia y el porcentaje aplicable en cada caso.

![](/media/image88.png)

Al dar de alta un Cuadro de Impuestos será necesario rellenar el campo Vigencia, mediante el que se definirá el periodo a partir del cual se activará el cuadro de impuestos definido.

Desde la pantalla de entrada de esta opción de menú, pulsando el botón CONSULTAR se podrán listar todos los Cuadros de Impuestos que se hayan dado de alta, indicando una vigencia y un tratamiento concreto y pulsando **“Consultar”:**

![](/media/image89.png)

Al Consultar se mostrarán los tipos de impuestos para el tratamiento identificado, indicando el porcentaje y el recargo en cada caso.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Cuadro de Impuestos:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro, una vez editado el registro, se utilizará el icono ![](/media/image19.png)

### \[PORTUGAL\] Comunicación Anual de las facturas emitidas (SAFT-PT) ![](/media/image90.png)

Desde esta opción de menú será posible realizar la generación del fichero XML asociado a las facturas emitidas en el rango de tiempo seleccionado por el usuario. El fichero generado será compatible con la versión 1.03\_01:

> ![](/media/image91.png)

### \[PORTUGAL\] Comunicación Mensual de las facturas emitidas (SAFT-PT) ![](/media/image90.png)

Desde esta opción de menú será posible realizar la generación del fichero XML asociado a las facturas emitidas en el rango de tiempo seleccionado por el usuario. El fichero generado será compatible con la versión 1.03\_01:

> ![](/media/image92.png)

## Configuración de la Tesorería

### Mantenimiento de Bancos ![](/media/image93.png)

Desde esta opción de menú, ubicada en **Administración -\> Tesorería,** se darán de alta los bancos con los que trabaja la empresa, así como los códigos de estos bancos.

![](/media/image94.png)

Aunque es recomendable rellenar todos los campos porque de este modo se recuperarán automáticamente en otros procesos de la aplicación, los únicos campos obligatorios son el código, la descripción y los días de fin de riesgo remesados.

El significado de los campos de la pantalla es el siguiente:

  - Código: puede ser hasta de 11 dígitos

  - Descripción: Nombre del Banco

  - Domicilio: Calle, número, oficina.

  - Población del banco.

  - Provincia.

  - Teléfonos de contacto.

  - Fax.

  - CCC: El CCC se dará de alta seguido, sin espacios ni guiones ni barras, ejemplo: 20980360150002005529.

  - CIF del banco.

  - CP de la localidad.

  - Observaciones: campo texto para insertar cualquier anotación a tener en cuenta.

Desde la pantalla de entrada a esta opción de menú se podrán listar todos los bancos pulsando el botón **Consultar.** Podrá filtrarse por código, descripción y registros activos.

Se listarán todos los bancos mostrando el código y la descripción.

![](/media/image95.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Banco:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

Haciendo click sobre la opción **“Imprimir**”, se llega a la siguiente pantalla en la que se muestran las distintas versiones del informe de listado de bancos:

![listado\_bancos](/media/image96.png)

### Mantenimiento de Tipos de Efectos ![](/media/image97.png)

Los tipos de efecto permiten agrupar los diferentes Medios de Pago y definir cuáles de ellos son al contado.

En este punto de menú se definirán los diferentes Tipos de Efecto que se vayan a utilizar, por ejemplo: Pagaré, Giro, Contado, Transferencia, etc. Posteriormente, en el Mantenimiento de Medios de Pago se asociará a cada forma de pago el Tipo de efecto que le corresponda.

![](/media/image98.png)

Los campos de la entidad Tipo de Efecto son los siguientes:

  - Código: puede ser alfanumérico de 2 dígitos.

  - Descripción: Nombre del Tipo de Efecto.

  - Remesable: si se gestiona a través de Remesas al banco.

  - Entrada Documento Automática: indica si es de Aceptación Automática, es decir, que no es necesaria la validación del cliente para el envío del documento al banco. Por ejemplo, esto ocurre con los Giros.

  - Activo: indica si el registro está activo u obsoleto.

Desde la pantalla de entrada a esta opción de menú se podrán listar todos los tipos de efectos pulsando el botón “**Consultar”.** Podrá filtrarse por código, descripción y registros activos.

![](/media/image99.png)

Los Resultados mostrarán el código y la descripción de cada registro.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Tipo de Efecto:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Conceptos de movimientos de caja ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\conceptosMovimentosCaja.png](/media/image100.png)

Desde este mantenimiento se pueden definir los conceptos que se van a asociar a los movimientos de caja. La búsqueda se podrá filtrar por código y descripción, además de por el estado de los conceptos existentes.

Además de dar de alta un concepto de movimiento de caja mediante el botón ![](/media/image16.png) Añadir de la cabecera, se puede editar un concepto existente con el icono![](/media/image17.png), consultar un concepto con el icono de la lupa ![](/media/image18.png) , o eliminarlo con el botón ![](/media/image19.png)

![](/media/image101.png)

Para definir un concepto de movimiento de caja se deben rellenar los campos:

  - Código: Valor alfanumérico único para cada concepto de movimiento de caja.

  - Descripción: Título descriptivo del movimiento de caja.

  - Activo: Check que indica si el concepto está activo y se puede asociar a un movimiento.

  - Manual: Check que indica si el movimiento se realiza de forma manual.

![](/media/image102.png)

### Mantenimiento de Medios de Pago ![](/media/image103.png)

En este punto de menú se definirán las formas de pago disponibles en la aplicación para que puedan utilizarse en los procesos de ventas y compras. Está ubicado dentro del menú **“Administración -\> Común”.**

El Mantenimiento de los Medios de Pago es muy importante para la gestión correcta de la Tesorería, ya que en función de la definición de éste Mantenimiento se generan los vencimientos.

![](/media/image104.png)

![](/media/image105.png)

La pantalla tiene dos bloques:

En el primer bloque se identifican los **“Datos del Medio de Pago”:**

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre del medio de pago.

  - Activo: si está en uso.

  - Recuento automático Caja.

En el segundo Bloque aparecen una o dos pestañas dependiendo de la forma de pago. En el caso de que la forma de pago sea al contado (esté chequeada la casilla “Contado”), no aparece la pestaña de **“Vencimientos”.** Si la casilla “Contado” no está chequeada sí aparece la pestaña de Vencimientos para indicarlos.

El significado de los campos es el siguiente:

1.  **Pestaña Datos Generales:** en el apartado <span class="underline">Modalidad</span> habrá que indicar si la forma de pago es Contado o no, si se chequea la casilla “contado” aparecerán dos campos para indicar el tipo de contado: Efectivo o Tarjeta de Crédito:

![](/media/image106.png) ![](/media/image107.png)

El campo Tipo de efecto será un campo de tipo ayuda que recuperará los Tipos de efectos dados de alta en el Mantenimiento de Tipos de Efecto (punto 4.3.2 de este manual). Los tipos de efecto servirán para agrupar los medios de pago, de forma que, por ejemplo, podrán existir los medios de pago: Pagaré a 30 días, Pagaré a 60 días, Pagaré a 90 días; y todos ellos tendrán asociado el Tipo de efecto Pagaré.

En el apartado <span class="underline">Visibilidad</span> se indica si el medio de pago es visible en los procesos de compras, ventas y en la tienda virtual. La casilla "Manual" permite al usuario indicar si ese medio de pago se aplicará de forma manual en los procesos de venta.

La casilla de Tienda Virtual sólo aparece en los medios de pago de contado, es decir, que esté chequeada la casilla **“Contado”.**

2.  **Pestaña Vencimientos:**

![](/media/image108.png)

Cuando la forma de pago no es contado, es necesario identificar los vencimientos. Para insertar o modificar un vencimiento, hay que editar primero (icono ![](/media/image17.png) de la cabecera) y se activará en el detalle el icono ![](/media/image16.png) para crear un nuevo vencimiento.

En el vencimiento se debe indicar:

  - Descripción: descripción general del vencimiento, por ejemplo “pagare 30, 60”

  - Nº de vencimientos: número de vencimientos que tendrá la modalidad de pago

  - Días de cadencia: número de días hasta el primer vencimiento

  - Días entre vencimientos: número de días entre vencimientos

  - Naturales: identifica si los días anteriores serán naturales o no.

**Ejemplo: Pagaré 30, 60**

  - Nº de vencimientos: 2

  - Días Cadencia: 30

  - Días entre vencimientos: 30

Desde la pantalla de entrada de esta opción de menú se podrán listar todas las formas de pago mediante el icono **“Consultar”.**

Se pueden establecer criterios de búsqueda opcionales utilizando los campos del código y descripción.

![](/media/image109.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Medio de Pago:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

### Configuración en comerzzia para el uso de tarjetas de regalo

Comerzzia permite realizar la configuración de dos tipos de tarjeta:

  - De importe fijo

  - De importe variable seleccionable en el momento de la compra.

La configuración de ambos tipos de tarjetas regalo se hará siguiendo los siguientes pasos:

1.  **Creación de los artículos asociados a las tarjetas regalo.** En función de la política de tarjetas de cada cliente, se crearán los artículos necesarios para modelar los tipos de tarjeta regalo que maneje. Esto se realizará desde el **“Mantenimiento de artículos”**, creando tantos artículos como tipos de tarjeta regalo de importe fijo tenga y/o un artículo genérico que definirá el tipo de tarjeta de importe variable. A modo de ejemplo, en nuestro caso hemos creado dos artículos, uno para las tarjeta regalo de importe fijo de 30 euros y otro para tarjetas regalo recargables en el momento de la venta:

![](/media/image110.png)

2.  **Configuración de los códigos de artículos asociados a las tarjetas regalo en cada POS de tienda:** Tras la creación de los artículos, se deberá acceder al fichero **“devices.xml”** de cada POS en el que se soporte la gestión de tarjetas regalo y configurar los códigos de artículos anteriores, tal como se explica de forma detallada en el **“Manual de Instalación en tienda”**. A modo de ejemplo, se muestra captura de pantalla de cómo debe visualizarse los artículos asociados desde el menú de configuración:

![](/media/image111.png)

3.  **Solicitud de las tarjetas regalo al fabricante:** En paralelo, se solicitarán las tarjetas al fabricante. Comerzzia permite la utilización de tarjetas regalo con código de barras o de banda magnética. No existe ningún tipo de limitación en relación a la codificación asociada a la tarjeta regalo.

4.  **Carga masiva de tarjetas en el sistema:** Tras la recepción de las mismas, estás se deberán cargar en el sistema a través de una operación masiva de carga de las mismas. Este proceso no está disponible actualmente desde el área de administración de comerzzia, por lo que deberá ser solicitado por el cliente.

**NOTA IMPORTANTE:** La gestión y mantenimiento de las tarjetas regalo así como la consulta de movimientos asociadas a las mismas desde el área de Administración de comerzzia solo está disponible tras la contratación del módulo Loyalty. En caso contrario, se podrá disponer de esta funcionalidad pero sin posibilidad de gestión por parte de los usuarios.

## Configuración de Artículos

### Mantenimiento de Familias ![](/media/image112.gif)

Las familias permiten agrupar los artículos según su clasificación.

Esto nos va a permitir realizar análisis y estadísticas no sólo por producto (artículo) sino también por familia.

Las familias se identifican como una agrupación de los artículos. En este apartado se darán de alta las familias para posteriormente asociar a cada artículo la familia a la que pertenece.

![](/media/image113.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de 6 dígitos.

  - Descripción: Nombre de la familia

  - Activo: identifica si el registro está en uso u obsoleto.

Desde la pantalla de entrada a esta opción de menú se podrán listar todas las familias utilizando el botón **Consultar.**

Se podrán establecer criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image114.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Familia:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

Al hacer click sobre el botón **“Imprimir”,** se tiene la siguiente pantalla en la que es posible seleccionar la versión del listado de familias que se desea imprimir.

![listado\_familias](/media/image115.png)

![](/media/image116.png)

### Mantenimiento de Categorizaciones ![](/media/image117.png)

Las categorizaciones son agrupaciones de artículos diferentes a la familia, a efectos de poder presentar los Artículos al público de forma diferente a cómo se organizan internamente en la propia empresa. Por ejemplo, para definir las diferentes categorías de AECOC.

Las categorías definidas en este punto de menú serán las que se tengan en cuenta en el comercio electrónico para las búsquedas de artículos (categorización a dos niveles), y en el POS (categorización a N niveles). El árbol de categorías se basa en la codificación de las mismas por grupo de dos dígitos, de forma que, por ejemplo, ‘01’ es una categoría raíz o de primer nivel, ‘0101’ y ‘0102’ son dos subcategorías (o de segundo nivel) de ‘01’, ‘010101’ y ‘010102’ dependen de ‘0101’, y así sucesivamente.

En este punto de menú se definirán las diferentes categorías que se quieran tener en cuenta para agrupar los artículos. Posteriormente en el Mantenimiento de artículos se asociará a cada artículo su categorización.

![](/media/image118.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 5 dígitos.

  - Descripción: Nombre de la categoría.

  - Activo: si está en uso u obsoleto.

  - Etiquetas: A partir de la versión 3.0.1 es posible añadir etiquetas a una categorización.

![](/media/image119.png)

Desde la pantalla de entrada a esta opción de menú se podrán listar todas las Categorizaciones utilizando el botón “**Consultar”.**

Se podrán establecer criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image120.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Categoría:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

Mediante el botón **“Imprimir”** es posible acceder a las distintas versiones del listado de Categorizaciones, tal y como se puede ver en las siguientes capturas de pantalla:

![listado\_categorizaciones](/media/image121.png)

![](/media/image122.png)

### Mantenimiento de Secciones ![](/media/image123.png)

La Sección permite crear agrupaciones de artículos que sirvan para organizar los productos en la tienda.

Ejemplos de Secciones podrían ser Carnicería, Lácteos, Perfumería, Droguería, etc.

En este punto se dan de alta las Secciones para posteriormente en el mantenimiento de artículos asociar a cada artículo la sección a la que pertenece.

![](/media/image124.png)

Los campos de la pantalla son los siguientes:

  - Código: Puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre identificativo de la sección

  - Ruta de preparación: La ruta de preparación sirve para orientar sobre la ubicación de la sección en la tienda para facilitar la preparación de pedidos. Es un campo opcional de la sección.

  - Activo: Identifica si el registro está en uso u obsoleto.

Desde la pantalla de entrada a esta opción de menú se podrán listar todas las Secciones utilizando el botón “**Consultar”.**

Se podrán establecer criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image125.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Sección:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Marcas

Los artículos pueden tener asociada una marca de forma opcional. Esto permite disponer de una organización de los mismos por marca, útil principalmente en la Tienda Virtual.

En este punto se dan de alta las Marcas para posteriormente en el mantenimiento de artículos tener la posibilidad de asociar cada artículo a su marca correspondiente.

![](/media/image126.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre identificativo de la sección

  - Fabricante: Fabricante asociado a la marca. Opcional.

  - Activo: identifica si el registro está en uso u obsoleto.

Desde la pantalla de entrada a esta opción de menú se podrán listar todas las Marcas utilizando el botón “**Consultar”.**

Se podrán establecer criterios de búsqueda utilizando los campos de Código, Descripción y Fabricante.

![](/media/image127.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Marca:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Artículos ![](/media/image128.png)

Desde la pantalla de entrada a esta opción de menú se pueden listar todos los Artículos utilizando el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código, Descripción, Familia, Proveedor y Categorización.

![](/media/image129.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Artículo:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

Desde este punto de menú deberán darse de alta todos los productos de la empresa.

![](/media/image130.png)

Aunque sólo son obligatorios los campos de código, descripción, impuesto y precio de costo, se recomienda rellenar todos los campos posibles que faciliten la automatización en los procesos de compras y ventas.

La pantalla se compone de dos bloques:

En el primer bloque de Datos del Artículo se identifican:

  - Código: puede ser alfanumérico de hasta 20 dígitos.

  - Descripción: Nombre del artículo

  - Activo: identifica si está en uso

El segundo bloque se compone de varias pestañas, visualizándose información diferente en función de la pestaña en que se posicione el usuario:

> **Pestaña de Datos Generales:** se compone de los siguientes apartados:

1.  **<span class="underline">Organización: </span>**

<!-- end list -->

  - Formato: el campo formato se emplea para definir aquellos artículos de peso variable. Si el campo se rellena con kg (no se distinguen mayúsculas de minúsculas) se considerará que el artículo es de peso variable, y al seleccionarlo desde el POS visualizaremos el campo “Peso”. La cantidad en estos artículos se determina con una balanza. Esta operativa sólo se hará en el caso de que hayamos configurado la balanza en el POS. Si la balanza no está configurada, la cantidad se toma del campo cantidad de la pantalla, pudiéndose introducir manualmente si el peso leído por la balanza de la caja es 0.

  - Familia: campo ayuda que recuperará las familias que se hayan dado de alta en el Mantenimiento de Familias. Se deberá seleccionar la familia a la que pertenezca el artículo.

  - Sección: Campo ayuda que recuperará las secciones que se hayan dado de alta en el Mantenimiento de Secciones. Se deberá seleccionar la sección que corresponda con el artículo.

  - Categorización: campo ayuda que recuperará las categorías que se hayan dado de alta en el Mantenimiento de Categorizaciones.

  - Marca: campo ayuda que recuperará las marcas que se hayan dado de alta en el Mantenimiento de Marcas.

  - Desglose 1 y Desglose 2: si se ha configurado la empresa para usar desgloses (por ejemplo tallas y Colores), aquí aparecerán estos campos, debiendo chequearlos si el artículo tiene Desgloses.

  - En escaparate: Este campo solo se mostrará cuando el artículo tenga una categoría asignada. En ese caso, si se chequea este campo, el artículo se visualizará “en primera instancia” en la Tienda Virtual.

  - Genérico: esta casilla se marcará en los artículos que no referencian a un producto en concreto, por ejemplo, para pequeño material del que no interesa dar de alta un artículo por cada elemento, sino que se da de alta un artículo genérico y es en los pedidos o albaranes donde se personaliza el nombre. Esto implica que no se realizará control de almacén para estos artículos. Un ejemplo serían tornillos pequeños.

  - Impuestos: campo ayuda que recuperará los tipos de Impuestos que se hayan dado de alta en el Mantenimiento de Tipos de Impuestos. A cada artículo habrá que asociarle el tipo de impuesto que le corresponda. Esta asociación es importante porque será uno de los datos que se utilice para calcular los impuestos en los procesos de Compras y Ventas.

  - Sustitución: campo tipo ayuda que recupera los tipos de sustitución que se hayan dado de alta en Preferencia de Sustitución en Pedidos. Determina el criterio de sustitución por defecto del artículo en caso de no encontrarse disponible en el momento de la preparación del pedido.

  - Tipo de artículo: variable binaria para definir si el artículo se vende por unidades o si se trata de un artículo de peso variable.

<!-- end list -->

2.  **<span class="underline">Compras: </span>**

Se compone de los siguientes datos:

  - Proveedor: campo ayuda que recuperará los proveedores que se hayan dado de alta en el Mantenimiento de Proveedores. El proveedor que se asocie en el artículo se corresponderá con el proveedor habitual.

  - Dto. Proveedor: este campo sirve para indicar el descuento que puede ofrecer el proveedor. Si se indica un descuento, éste será contemplado en los procesos de compras de manera que al añadir el artículo a un pedido o un albarán se establecerá el descuento al valor indicado; si no se introduce descuento, el valor por defecto será cero.

  - Referencia: campo texto para insertar la referencia del artículo para el proveedor.

  - Fabricante: campo ayuda que recuperará los proveedores que se hayan dado de alta en el Mantenimiento de Proveedores con el Tipo Fabricante.

<!-- end list -->

3.  **<span class="underline">Precios:</span>**

**Todos los artículos estarán dados de alta en la tarifa general, al dar de alta el artículo, los datos del apartado Precios de la pestaña de Datos Generales se guardarán automáticamente en la tarifa GENERAL.** (Para más información sobre Tarifas consultar el punto Mantenimiento de Tarifas de este Manual).

El significado de los campos del apartado “Precios” de Datos Generales del artículo son los siguientes:

  - Precio Costo: identifica el precio de costo del artículo del proveedor. Esto permitirá que al realizar un pedido de compras se recupere automáticamente el precio del artículo.

  - Act. Automática al comprar: si se chequea esta casilla, el precio de costo del artículo se actualizará automáticamente con el último precio de compra del último albarán al proveedor.

  - Ult. Actualización: indica la fecha y hora en que se produjo el último cambio en el precio de costo.

  - Factor marcaje: permite calcular el precio de venta a partir de multiplicar el precio de compra por este factor de marcaje (margen que se quiere obtener con respecto al precio).

  - Precio marcaje: si se rellena este campo, será el que se utilice como precio de venta. Factor aplicado: campo calculado, que identifica el porcentaje directo sobre el precio de costo que se está obteniendo de margen, en función del precio de venta.

  - Precio marcaje + impuestos: corresponde a la suma del precio marcaje y los impuestos.

  - Factor aplicado: campo calculado, es el %MV (porcentaje de margen de ventas), sobre PVP.

  - Precio de venta: campo calculado, identifica el precio de venta bruto con 4 decimales, sin impuestos.

  - Precio de venta + impuestos: campo calculado, identifica el precio de venta neto redondeado a 2 decimales, con impuestos.

**Por** **ejemplo:**

  - **Se identifica un porcentaje de marcaje:** supongamos que tenemos un precio de costo de 100 y se define un porcentaje de marcaje de 10 (margen sobre precio de costo); el precio de venta será:100/(1-0,1)=111,1111

  - **Se identifica un precio de marcaje:** supongamos que tenemos un precio de costo del artículo de 10 y se define un precio de marcaje de 20; el factor aplicado se calculará automáticamente como 50, que reflejaría que se está obteniendo el 50% de margen con respecto al precio de costo. En este caso el precio de venta se establece automáticamente por el precio de marcaje, incluyendo 4 decimales, por lo que en este caso sería 20,0000.

<!-- end list -->

4.  **<span class="underline">Etiquetas: </span>**

La posibilidad de asociar etiquetas a artículos está disponible a partir de la V.3.0.1 de comerzzia. Mediante esta utilidad, es posible disponer de un conjunto de etiquetas identificativas del artículo, que podrán ser utilizadas tanto en la tienda virtual como en la generación de promociones de venta.

Se podrán tanto asociar etiquetas existentes, como crear nuevas etiquetas. Cuando se comienza a introducir la primera letra, el sistema de forma automática verificará si existen etiquetas que comiencen por dicha letra y las propondrá al usuario, pudiendo elegir entre utilizar la existente o crear una nueva. Si se crea una nueva pasará a estar disponible para el resto de artículos.

En los artículos con diferentes modo de preparación, éstos se parametrizan como etiquetas que deben pertenecer a la categoría MODOS DE PREPARACIÓN, la cual debe ser dada de alta desde el Mantenimiento de Categorías de Etiquetas.

NOTA: Para que a posteriori esta etiqueta pueda ser utilizada en otros aplicativos de comerzzia, es necesario asegurarse de que la etiqueta esté asociada a una categoría de etiquetas, desde el mantenimiento correspondiente. Por este motivo, se aconseja la creación de las etiquetas de forma previa a su asignación, utilizando para ello el “Mantenimiento de Categorías de Etiquetas” y el “Mantenimiento de Etiquetas” ubicado en el menú “Común”.

> **Pestaña de Observaciones: **

![](/media/image131.png)

Campo texto donde se podrán hacer anotaciones o insertar otra información relevante acerca del artículo.

> **Pestaña Código Barras: **

![](/media/image132.png)

Desde este punto se insertan los diferentes códigos de barras del artículo.

Pinchando en el icono ![](/media/image16.png) se podrá añadir un nuevo código de barras. Si existen desgloses (por ejemplo tallas y colores) deberá indicarse el desglose, si no existe desglose en este campo se deberá poner un \* (asterisco).

El código de barras puede ser introducido manualmente si el artículo lo tiene o bien puede ser generado automáticamente pulsando en el icono ![](/media/image133.png)

Si el código de barras se corresponde con un DUN14 (Cajas) se marcará la casilla DUN14.

Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

  - **Pestaña Unidades de Medida: **

![](/media/image134.png)

Desde este punto se insertan las diferentes unidades de medida para el artículo.

Lo primero será seleccionar la **Etiqueta:**

  - Unidad: unidad de medida en la que se expresa la etiqueta. Es un campo ayuda que recuperará los valores dados de alta en el Mantenimiento de Unidades de Medida de Etiquetas.

  - Cantidad: cantidad que se corresponde con la unidad de ese artículo. Hay que considerar el factor de la unidad de medida seleccionada.

> **Ejemplo:** Lata de leche condensada de 370gr. Se quiere mostrar el precio por kilo. El factor de la unidad de medida KILO es 1000 (relación entre el kilo y el gramo, que es la unidad más común en el sector alimentación).
> 
> ![](/media/image135.png)

En el Bloque de **Unidades de Medida** se podrán realizar las siguientes acciones:

  - Indicar una Unidad de Medida alternativa: en este caso, todas las cantidades de los almacenes se expresarán también en esta unidad de medida.

  - Se podrán dar de alta Unidades de Medida diversas para el artículo, de forma que en los pedidos se puedan utilizar estas unidades, realizando la conversión a la unidad de medida de la etiqueta del artículo. Para cada unidad de medida se podrá identificar el Alto, Ancho, Fondo y Peso.

**Ejemplo:** El artículo “AVESTRUZ AL QUESO MI CONSERVA LATA 225 GR”: la unidad de medida de la etiqueta serían Kilos, la cantidad en la unidad del artículo serían 225 (GR). Además, existen las Unidades de Medida: UNID (UNIDAD) que equivale a 1 lata de “AVESTRUZ AL QUESO MI CONSERVA LATA 225 GR”; CAJA que equivale a 24 latas de “AVESTRUZ AL QUESO MI CONSERVA LATA 225 GR” y PALE que equivale a 1344 latas de “AVESTRUZ AL QUESO MI CONSERVA LATA 225 GR”.

![](/media/image136.png)

El campo Peso en este caso es opcional, y sólo aparece con carácter informativo. Sin embargo, en productos de peso variable que se vendan por unidades este campo es necesario para ofrecer al cliente el importe a pagar.

![](/media/image137.png)

  - **Pestaña Almacenes:**

![](/media/image138.png)

En este apartado se recuperarán a nivel informativo los datos de stock del artículo en los almacenes. Además se podrá insertar un stock mínimo y máximo. Los campos que se muestran son los siguientes:

  - Código: mostrará el código del almacén. Si el artículo estuviera en más de un almacén se mostrará una línea por almacén.

  - Desglose 1 y Desglose 2 (por ejemplo tallas y colores): en los casos que existan desgloses el stock se mostrará por artículo y por desgloses, visualizándose líneas diferentes por almacén y desglose.

  - Stock: mostrará a modo informativo el stock actual del artículo en los almacenes.

  - Stock Unidad Medida Alt.: mostrará a modo informativo el stock existente según la unidad alternativa de medida del artículo. Previamente ésta se deberá haber indicado en la Pestaña de Unidades de Medida.

  - Stock Mínimo: será un campo que podrá editarse para insertar el stock mínimo del artículo que debe haber en el almacén para que no se produzca “rotura de stock”, y que tendrá la utilidad de poder utilizarlo posteriormente en los procesos de compras por stock mínimo.

  - Stock Máximo: será un campo que podrá editarse e insertar el stock máximo del artículo a nivel informativo, por ejemplo para indicar a partir de qué stock se incurriría en costes por almacenaje de producto.

  - Stock Pte. De Recibir: muestra a nivel informativo el stock que está en pedidos de compras pendientes de albaranear.

  - Stock Pte. Servir: muestra a nivel informativo el stock que está en pedidos de venta pendientes de albaranear.

  - Acciones: permite consultar ![](/media/image18.png) los datos en modo ficha. Para volver al modo tabla habrá que pinchar el icono ![](/media/image139.png)

  - **Pestaña Tarifas: **

![](/media/image140.png)

  - Desde esta pestaña del Mantenimiento de Artículos se podrán consultar las tarifas en las que esté incluido el artículo, así como las promociones, visibles en el segundo bloque.

Pinchando en el icono ![](/media/image18.png) se visualizarán los datos de la tarifa en modo ficha. Se podrán modificar directamente datos de precios de las tarifas directamente desde esta pantalla pinchando en el icono![](/media/image17.png). (Para que se visualice Editar en detalle, primero será necesario Editar la pantalla con el icono de la cabecera).

  - **Canales:**

![](/media/image141.png)

Esta pestaña está disponible desde la v 3.0.1 de comerzzia.

Desde esta pestaña se podrán asociar los artículos a los canales de venta que proceda.

Pinchando en el icono ![](/media/image18.png) se visualizarán los datos del canal de venta asociado en modo ficha. Para desasociar un artículo de un canal de venta se utilizará el icono![](/media/image19.png). Para poder realizar esta operación primero será necesario Editar la pantalla con el icono de la cabecera.

#### Asistente para el Alta Rápida de Artículos ![](/media/image142.png)

Para facilitar el alta masiva de Artículos existe la opción ![](/media/image142.png) Alta Rápida en la cabecera de la pantalla de Mantenimiento de Artículos. Esta opción permite dar de alta artículos con la información mínima obligatoria.

Está orientado al alta secuencial de Artículos semejantes, donde la pantalla propone el código del Artículo y mantiene, por defecto, los datos entre un registro y el anterior

![](/media/image143.png)

#### Impresión de Informes asociados a Artículos

![](/media/image144.png)

Desde la operación “Imprimir” ubicada en las opciones de la cabecera de la pantalla de consulta, accedemos a una pantalla de lanzamiento de informes que incluye diferentes condiciones de filtrado para la generación de informes. Los informes disponibles de estándar son los siguientes:

  - Listado de Artículos.

  - Impresión de etiquetas de artículos.

  - Listado de artículos exportables.

![](/media/image145.png)

### Mantenimiento de Productos ![](/media/image146.gif)

En entornos de NON-FOOD, los productos en comerzzia son artículos o conjunto de artículos que pertenecen a una misma marca, categoría, etc, pero que tienen formatos de venta diferentes.

*Ejemplo:* La colonia *Hugo Boss* es un **producto** único compuesto por los diferentes **artículos**, con diferentes precios, relativos a los diferentes formatos en que se vende el producto: *Hugo Boss 50ml, Hugo Boss 100ml,…*

El buscador de productos de backoffice permite filtrar por código, descripción, marca y categoría.

![](/media/image147.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Producto:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un producto en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

Para dar de alta un producto, se debe definir:

  - Código: Identificador único del producto.

  - Descripción: Título descriptivo del producto.
    
    **Pestaña Datos Generales:**
    
      - Marca: Campo ayuda que tira de las marcas definidas en el Mantenimiento de Marcas para asignarle la marca correspondiente al producto.
    
      - Impuesto: Campo ayuda que tira de los tipos de impuestos dados de alta en el Mantenimiento de Tipos de impuestos para concretar el tipo de impuesto sobre el producto.
    
      - Categoría: Campo ayuda para definir la categoría a la que pertenece el producto.
    
      - Observaciones: Campo de texto libre para aclaraciones u observaciones del producto.
    
      - Etiquetas: Campo que permite la asignación de etiquetas al producto.

![](/media/image148.png)

**Pestaña Artículos:**

Desde la pestaña Artículos se permite añadir el/los artículo/s asociados al producto.

![](/media/image149.png)

**Pestaña Canales:**

Desde la pestaña Canales se definen los canales de venta en los que se comercializa el producto.

![](/media/image150.png)

### Mantenimiento de Unidades de Medida ![](/media/image151.gif)

Con el fin de facilitar la gestión de las unidades de medida, comerzzia incluye un nuevo mantenimiento que permite consultar las unidades de medida disponibles y dar de alta nuevas unidades, así como la edición y la eliminación de las mismas.

![](/media/image152.png)

Cada unidad de medida se define con un código identificador y una descripción. Además, se puede añadir adicionalmente una prioridad de la unidad de medida. Dicha prioridad se establecerá a nivel de artículo desde el **Mantenimiento de artículos**, cuando se le asigne la unidad de medida de venta.

![](/media/image153.png)

### Mantenimiento de Unidades de Medida de Etiquetas ![](/media/image154.png)

En este punto de menú se darán de alta las unidades de medida que van a mostrar en la etiqueta del artículo.

![](/media/image155.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 4 dígitos.

<!-- end list -->

  - Descripción: descripción general de la unidad de medida.

  - Descripción de Etiqueta: descripción que va a figurar en la etiqueta del artículo.

  - Factor: equivalencia en la unidad de medida base del artículo que se utiliza para calcular el precio.

Por **ejemplo**, para productos de alimentación, una de las medidas que se utilizan son los KILOS, que en la etiqueta deben aparecer como Kg. Para calcular el precio se establece la equivalencia en gramos (1000).

Desde la pantalla de entrada a esta opción de menú se pueden listar todas las Unidades de Medida utilizando el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image156.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Unidad de Medida:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Preferencia de Sustitución en Pedidos ![](/media/image157.gif)

Desde el backoffice de comerzzia se permite establecer criterios de sustitución de artículos en el caso de que no estén disponibles en el momento de la preparación del pedido. Desde esta área del menú se permite consultar los criterios de sustitución en pedidos, filtrando por código o descripción.

![](/media/image158.png)

Además, será posible realizar el Alta/Edición/Consulta/Baja de un criterio de sustitución:

  - Para dar de alta un registro hay que pulsar sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para suprimir un registro en concreto se debe hacer click sobre el icono![](/media/image19.png)

Los campos a rellenar para definir un criterio de sustitución son:

![](/media/image159.png)

  - Código: Valor alfanumérico único para cada criterio de sustitución.

  - Descripción: Título descriptivo del criterio de sustitución.

  - Artículo de sustitución de la misma marca: Variable tipo char (1) que indica si el criterio implica mantener la misma marca.

### Mantenimiento de Tipos de Embalaje ![](/media/image160.gif)

Desde este mantenimiento se permite consultar los diferentes tipos de embalaje disponibles para la entrega de productos.

![](/media/image161.png)

Desde este mantenimiento se permite realizar el Alta/Edición/Consulta/Baja de un tipo de embalaje:

  - Para dar de alta un registro hay que pulsar sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para suprimir un registro en concreto se debe hacer click sobre el icono![](/media/image19.png)

La configuración de un nuevo tipo de embalaje requiere un código identificador único para cada tipo de embalaje y una descripción. Adicionalmente, se puede asociar un artículo al tipo de embalaje si éste va a formar parte de la venta.

![](/media/image162.png)

## Configuración de Almacenes

### Mantenimiento de Tipos de Servicios

Los servicios de comerzzia se clasifican según el tipo de servicio al que pertenecen, los cuales son definidos mediante el mantenimiento de tipos de servicios. En la versión 4.0 de comerzzia, se contemplan diversos tipos de servicios relacionados con la venta en tienda física y en tienda online.

La búsqueda de los tipos de servicios se puede filtrar por código y por descripción.

![](/media/image163.png)

Desde esta ventana se puede:

  - Dar de alta un nuevo tipo de servicio, pulsando sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar un tipo de contacto utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar un registro en concreto haciendo ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png)

Para definir un tipo de servicio deben rellenarse los siguientes campos:

![](/media/image164.png)

  - Código: Variable alfanumérica, debe ser única para cada tipo de servicio.

  - Descripción: Título descriptivo identificativo del tipo de servicio.

  - Importe mínimo compra: A veces se requiere un importe mínimo de compra para ofrecer determinados servicios. Si no se precisa, el campo debe rellenarse con valor 0.

  - Ámbito aplicación: Descripción de la casuística que da lugar a la aplicación de un servicio del tipo en cuestión.

  - Selección manual: Selector que se marca para indicar si el cliente final puede elegir que se le sirva un servicio de este tipo.

  - Logística interna: Selector que se marca para indicar que el tipo de servicio requiere logística interna por parte de la empresa.

  - Logística externa: Selector que se marca para indicar que el tipo de servicio requiere logística externa.

  - Requiere pago: Selector que se marca para indicar que el tipo de servicio requiere el pago por parte del cliente final.

  - Requiere preparación: Selector que se marca para indicar que el tipo de servicio requiere preparación por parte de personal de la organización.

  - Código tipo de servicio logística interna: Indica el código del tipo de servicio al que se dirige la logística interna, si procede.

  - Proceso de estados: Indica el proceso de estados que seguirá un servicio de este tipo.

  - Portes: Los tipos de servicios pueden tener asociados tipos de porte por defecto. Además, el tipo de porte de un servicio se podrá definir a nivel de servicio-tienda, tomándose el tipo de porte del tipo de servicio en el caso de que no se defina otro a nivel inferior.

### Calendarios de Servicios ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\actualizacion.gif](/media/image165.gif)

En comerzzia se requiere la definición de calendarios de servicios para que éstos sean asociados a los servicios que ofrece una tienda.

La búsqueda de calendarios de servicios definidos se puede filtrar por código y por descripción.

![](/media/image166.png)

Desde esta pantalla se acceden a las funcionalidades:

  - Crear un nuevo calendario de servicio, pulsando sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar un calendario utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar un registro en concreto haciendo ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Visualizar el calendario pulsando sobre ![Ver calendario](/media/image167.gif)

  - Dar de baja un registro mediante el icono![](/media/image19.png)

![](/media/image168.png)

Para dar de alta un nuevo calendario de servicio se requieren como campos obligatorios:

  - **Código:** Identificador único para cada calendario de servicio.

  - **Descripción:** Título descriptivo del calendario de servicio.

Además, los calendarios de servicios se componen de periodos de tiempo que determinan cuándo se ofrece el servicio. Estos periodos se pueden definir por:

  - **Semanas:** Cuando la franja horaria definida se repite en las mismas condiciones semana a semana.

  - **Fecha:** Hace referencia a días concretos en los que el servicio tiene sigue un calendario diferente al habitual o no se ofrece, como días festivos, etc.

Para la definición de una nueva franja horaria del calendario de servicios se debe pulsar previamente sobre el botón ![](/media/image17.png)Editar de la cabecera. Los campos obligatorios para cada franja horaria son:

![](/media/image169.png)

  - **Día de la semana/Fecha:** Indica qué día de la semana aplica la nueva franja horaria, o la fecha si se refiere a un día concreto. Si estamos en la opción de semana, es posible especificar los días de la semana para los que se aplicará el horario definido, permitiendo agilizar la creación de calendarios de servicio.

  - **Hora desde:** Hora de inicio de la franja horaria.

  - **Hora hasta:** Hora de fin de la franja horaria.

  - **Número máximo de pedidos:** Capacidad máxima del servicio en la franja horaria.

  - **Minutos de cadencia entre pedidos:** Parámetro que determina con cuanta antelación debe hacerse un pedido para que pueda ser servido en la franja horaria correspondiente.

> **Ejemplo**: Para que un pedido se pueda servir en la franja horaria de la tarde, de 16:00 a 20:00, debe recibirse la orden de pedido antes de las 14:00. Por tanto, se deberán fijar 120 minutos en la cadencia de la franja horaria.

### Mantenimiento de Tipos de Portes ![](/media/image170.gif)

Desde el mantenimiento de tipos de portes se permite:

  - Dar de alta un nuevo tipo de porte, pulsando el botón ![](/media/image16.png) Añadir de la cabecera.

  - Editar un tipo de porte existente utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar un registro en concreto o con el icono ![](/media/image18.png) o pulsando sobre la descripción del tipo de porte.

  - Eliminar un tipo de porte mediante el icono![](/media/image19.png).

![](/media/image171.png)

Para definir un tipo de porte se debe detallar una descripción y un artículo asociado al tipo de porte que se empleará para determinar el importe del porte. Adicionalmente, se debe fijar un importe mínimo de la venta, lo que permite establecer que se ofrezcan diferentes tipos de portes en función del volumen de venta. Además, se puede complementar la información con la URL de seguimiento facilitada por la empresa de reparto.

![](/media/image172.png)

Los tipos de portes se asignarán a un tipo de servicio desde el mantenimiento de tipos de servicios, o a un tipo de servicio ofrecido por una tienda desde el mantenimiento de tiendas, donde se permite asignar diferentes tipos de portes a diferentes zonas de cobertura del servicio.

### Mantenimiento de Almacenes ![](/media/image173.png)

Desde este punto de menú se podrán gestionar los almacenes de la empresa, tanto los que estén en la/s tienda/s como los que se encuentren en otra Ubicación.

Para listar los almacenes se deberá pulsar el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image174.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Almacén:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

Desde este punto de menú se darán de alta los almacenes de la empresa, tanto los que estén en la/s tienda/s como los que se encuentren en otra Ubicación.

![](/media/image175.png)

Aunque es conveniente rellenar todos los campos, los únicos campos obligatorios son el código, la descripción y la empresa.

Los campos de la pantalla son los siguientes:

  - Empresa: Empresa a la que se encuentra asociado el almacén.

  - Cliente: cada almacén debe tener asociado un cliente, de forma que cuando se hagan operaciones entre almacenes, por ejemplo, peticiones de una tienda, devoluciones o traspasos entre almacenes, se utilizará el cliente asociado al almacén para realizar la operación y se usará la tarifa de ese cliente. Cuando se da de alta un almacén, si no se rellena el campo cliente, al aceptar ![](/media/image176.png) para grabar el registro, la aplicación preguntará si se desea crear un cliente automáticamente con los datos del almacén:

> ![](/media/image177.png)

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: nombre identificativo del almacén.

  - Domicilio, Población, Provincia, Código Postal: correspondientes a la ubicación física del almacén

  - Teléfonos y Fax

  - Persona de Contacto

### Mantenimiento de Tiendas ![](/media/image178.png)

En la opción de menú de Mantenimiento de Tiendas podrán listarse todas las tiendas pulsando el botón “**Consultar”.**

![](/media/image179.png)

También es posible filtrar la consulta por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Tienda:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera. También será posible dar de alta tiendas a través del asistente, tal y como se comenta en el apartado siguiente de este manual.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

> Desde este punto de menú se darán de alta las tiendas de la empresa, entendiendo por Tienda como los diferentes establecimientos que existen con venta al público. Al dar de alta la tienda se creará automáticamente un almacén con el mismo código que la tienda.

![](/media/image180.png)

Los campos de la pantalla son los siguientes:

#### Pestaña General

> **Datos de la Tienda:**

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre de la Tienda.

  - Activo: si está en uso.

> **Datos de Contacto:**

  - **Cliente:** la tienda debe existir como Cliente, de forma que en las operaciones entre tiendas se utilizará ese cliente. Si al crear una tienda no se rellena el campo Cliente, la aplicación preguntará si se desea que se cree el registro automáticamente:

> ![](/media/image177.png)

  - **Empresa:** Empresa a la que se encuentra asociada la tienda.

<!-- end list -->

  - **Otros datos: Persona de contacto, domicilio, población, provincia, código postal, teléfonos y fax.** Además, a partir de los datos de la dirección se puede geolocalizar la posición para obtener la **ubicación** (longitud y latitud) y mostrar la posición de la tienda en el mapa.

> **NOTA:** El Código Postal es **obligatorio** en la parametrización de tiendas que sean almacenes preparadores de pedidos de la tienda online.
> 
> **Datos por defecto para la venta**
> 
> Cada tienda deberá tener asociado un **Concepto de Almacén**, que se usará en los documentos generados a partir de las ventas de las tiendas; un **Medio de Pago** para las ventas que se realicen en la tienda; también otros dos medios de pago para **Apartados** y **Promociones**, los cuales serán usados por el POS en apartados y promociones (consultar el manual del POS para más información sobre apartados y promociones). En esta sección se define también el **Canal de Venta** de la tienda y un **Calendario de Servicios** que determina el **calendario de apertura** de la tienda.
> 
> **Tipo de Tienda**
> 
> Los tipos de tienda son:

  - Online: trabaja directamente con los datos de la central

  - Offline: tiene su propia base de datos, y por lo tanto requiere de procesos de sincronización. Los métodos de sincronización disponibles definirán los tipos de tienda y se explican en detalle en este manual.

> **Versión de artículos**
> 
> Ofrece, en modo consulta, la versión actual de Artículos y la última revisada por la tienda. Esta comparación permite ver el grado de actualización que tienen las ventas en relación a posibles cambios realizados.

  - En modo edición, es posible forzar el envío de todos los artículos existentes en la central a través del icono![](/media/image181.png). Tras esta operación, se debe iniciar el proceso de sincronización para enviar todos los artículos a la tienda.

#### Pestaña Tarifas

![](/media/image182.png)

En este apartado se insertarán todas las tarifas que se utilicen en la tienda.

Siempre existirá la tarifa GENERAL donde estarán todos los artículos.

Al igual que para la versión de artículos, se podrá forzar el envío de los datos de la tarifa en la próxima sincronización a través del icono![](/media/image181.png).

#### Pestaña Configuración

![](/media/image183.png)

Esta pestaña solo tendrá datos en el caso de que la tienda sea del tipo OFF-LINE Centralizada. En este apartado se identificarán los datos a través de los cuales el Sincronizador de la Central se conectará con la tienda. El campo Parámetros indica un conjunto de parámetros que permite una configuración adicional en la conexión con la base de datos de la tienda. En el caso de tratarse de MySQL, por defecto se indican los parámetros mostrados en esta pantalla, que configuran un timeout de conexión de 30 segundos.

Es posible consultar el archivo xml asociado a esta configuración pulsando sobre el botón “Ver XML”.

#### Pestaña Usuarios

![](/media/image184.png)

En este apartado se insertarán todos los usuarios definidos para la Tienda. Todos ellos podrán interactuar con la Tienda.

#### Pestaña Cajas

![](/media/image185.png)

Desde esta pestaña se podrán gestionar las distintas cajas pertenecientes a la tienda. También existe la posibilidad de descargar el fichero de configuración de cada caja desde la acción![](/media/image186.png).

La acción ![](/media/image187.png) permitirá descargar el archivo de instalación del POS completo.

La acción ![](/media/image188.png) permitirá forzar la actualización de tarifa en la caja seleccionada.

Cuando se esté editando una tienda, tendremos la posibilidad de desactivar (![](/media/image189.png)), activar (![](/media/image190.png)), eliminar (![](/media/image191.png)) o dar de alta una nueva caja (![](/media/image192.png)), según se aprecia en la siguiente imagen:

![](/media/image193.png)

Para dar de alta nuevas cajas, se deben seleccionar aquellas cajas que estén disponibles del listado de cajas:

![](/media/image194.png)

Tras aceptar la operación, las cajas seleccionadas estarán asociadas a la tienda.

#### Pestaña Servicios

Desde la pestaña de servicios se accede al listado de los diferentes tipos de servicio que ofrece la tienda. Tras pulsar en el botón ![](/media/image17.png)Editar de la cabecera se accede al modo edición, donde se permite la asignación de un servicio a la tienda, la eliminación de un servicio, o la modificación de un servicio asignado previamente a la tienda.

Los servicios asociados a una tienda pueden tener asignados un calendario de servicio, en el caso de que el servicio se rija por un mismo calendario en toda su área de cobertura. La zona donde una tienda ofrece un determinado servicio se define mediante los códigos postales, en la pantalla de detalle del servicio. Además, se debe definir qué almacén es el encargado de preparar el pedido, en el caso de que la tienda ofrezca un servicio que requiera preparación.

![](/media/image195.png)

En el ejemplo de la imagen, la tienda se encarga de preparar los pedidos hechos en la propia tienda (servicios 0020 y 0030) y además ofrece un servicio de entrega de pedidos hechos y preparados en una tienda central (servicio 0040).

El campo Almacén de preparación tira de una ayuda con las tiendas existentes, pudiéndose seleccionar la propia tienda que se está parametrizando. Este campo es obligatorio para servicios que requieran preparación (ver Mantenimiento de Tipos de Servicios de este manual).

![](/media/image196.png)

En el caso de que un mismo servicio se ofrezca en diferentes áreas con diferentes coberturas (por ejemplo, reparto a domicilio local a diario y fuera de la localidad cada dos días), es posible determinar varios calendarios para un mismo servicio en función de los códigos postales donde dan cobertura. Esto se hace desde la pantalla de detalle de un servicio asignado a una tienda.

![](/media/image197.png)

Para asignar un nuevo código postal al área de cobertura de un servicio de una tienda, se debe acceder al modo edición de la pantalla mediante el botón ![](/media/image17.png)Editar y posteriormente pulsar en ![](/media/image16.png). La información a cumplimentar es el país y código postal como campos obligatorios, y calendario de servicio y tipo de porte como opcionales.

#### Pestaña Medios de Pago

En la pestaña Medios de Pago de una tienda se parametrizan todos los medios de pago aceptados por la tienda.

![](/media/image198.png)

Los medios de pago se muestran en una rejilla, pudiéndose añadir ![](/media/image16.png) o eliminar ![](/media/image191.png) medios de pago desde el modo de edición (![](/media/image17.png)Editar en la cabecera).

#### Asistente de Alta de Tiendas

Mediante el botón ![](/media/image16.png)Añadir existe la posibilidad de dar de alta tiendas a través de un asistente en el que se rellenarán los datos obligatorios de la tienda.

1.  Introducción de los datos generales de la Tienda:

![](/media/image199.png)

2.  Introducción del tipo de tratamiento de impuestos asociado a la Tienda:

![](/media/image200.png)

3.  Introducción de la tarifa asociada a la Tienda:

![](/media/image201.png)

4.  Selección del Tipo de Sincronización de la Tienda con la Central:

![](/media/image202.png)

  - En el caso de tipo de tienda **“OFF-LINE con Sincronización Centralizada”** requiere del detalle de parámetros de configuración:

> ![](/media/image203.png)

  - El resto de casos de tipos de tienda no requieren parámetros de configuración:

![](/media/image204.png)

5.  Selección de los usuarios asociados a la Tienda:

![](/media/image205.png)

6.  Selección de las cajas asociadas a la Tienda:

![](/media/image206.png)

1.  Finalización del proceso de alta de una Tienda:

![](/media/image207.png)

### Mantenimiento de Grupos de tiendas ![](/media/image208.gif)

Comerzzia permite organizar las tiendas por grupos y organizar los mismos de acuerdo al tipo de grupo. El objetivo del mantenimiento de grupos de tiendas es facilitar la organización de las diferentes tiendas de la compañía.

La búsqueda de grupos de tiendas se puede hacer filtrando por código y por descripción.

![](/media/image209.png)

Para dar de alta un nuevo grupo de tiendas se deben rellenar los siguientes campos:

![](/media/image210.png)

  - Código: Identificar único para cada grupo de tiendas.

  - Descripción: Título identificativo del grupo de tienda.

  - Tipo de grupo: Campo alfanumérico en el que guardar el tipo del grupo de tiendas.

  - Activo: Permite definir cuando un grupo de tiendas se encuentra activo/inactivo.

  - Tiendas del Grupo: Para añadir tiendas al grupo se emplea un buscador a partir del cual se tiene acceso al listado de tiendas. Posteriormente, se emplea un selector y se pulsa aceptar ![](/media/image176.png) para decidir qué tiendas forman parte del grupo.

![](/media/image210.png)

Las tiendas seleccionadas posteriormente se muestran en una rejilla, pudiendo ser eliminadas del grupo desde la misma.

La gestión de grupos de tiendas desde backoffice sigue la misma línea que en el resto de mantenimientos de comerzzia.

  - Para añadir un nuevo grupo de tiendas se selecciona ![](/media/image16.png) Añadir

  - Para editar la información de un grupo de tiendas existente se hace click en ![](/media/image17.png)

  - Para consultar un grupo de tiendas se pulsa sobre el icono ![](/media/image18.png)

  - Para suprimir un grupo de tiendas hay que pulsar en el icono ![](/media/image19.png)

### Mantenimiento de Conceptos de Almacenes Regularización ![](/media/image211.png)

Permite definir diferentes conceptos o motivos por los que sea necesario realizar una Regularización de almacén.

En este punto de menú se darán de alta los conceptos o motivos que se quieran contemplar en las Regularizaciones de almacén, de forma que, posteriormente, al dar de alta una Regularización de almacén, uno de los campos que se establecerá será el concepto por el que se realiza la Regularización.

![](/media/image212.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre del concepto.

  - Signo: si permite sólo signos positivos, sólo negativos o ambos (en este caso, el campo estará en blanco)

  - Almacén de destino: se puede establecer el almacén de destino mediante la ayuda correspondiente.

  - Visible Tiendas: si se quiere que el concepto se pueda utilizar en las Tiendas.

  - Activo: si se puede utilizar.

Desde la pantalla de entrada a esta opción de menú se pueden listar todos los almacenes utilizando el botón de “**Consultar”.**

Es posible también restringir los criterios de búsqueda utilizando los campos de Código y Descripción.

![](/media/image213.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de una Regularización:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

### Mantenimiento de Conceptos de Almacenes para Ventas ![](/media/image214.png)

La posibilidad de automatizar determinados criterios que se produzcan al realizar un pedido de Ventas.

En este punto de menú se darán de alta los conceptos que se quieran contemplar posteriormente en los procesos de ventas. Por ejemplo: Venta Directa, Venta a Tiendas, Devoluciones, etc.

![](/media/image215.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: Nombre del concepto.

  - Signo: Se permitirá seleccionar entre (+) Positivo, (-) Negativo o () Sin Signo.

  - Operación almacén: Vendrá condicionado por el signo seleccionado, tomando los valores: Entrada, Salida o No aplica.

  - Almacén Origen: para predeterminar el almacén de origen a través de la ayuda correspondiente.

  - Almacén destino: para predeterminar el almacén de destino recurriendo a la ayuda de almacenes.

  - Aceptación Automática de Pedidos: si se chequea esta casilla el Pedido de Venta no contemplará el estado PENDIENTE DE ACEPTACIÓN. De forma que pasará directamente del estado SOLICITUD DE PEDIDO al estado EN PREPARACIÓN.

  - Generación Automática de Pedido de Faltas: si se chequea esta casilla, para Pedidos de Venta, en el caso de que la cantidad pedida y la cantidad servida sean diferentes se generará automáticamente un pedido de faltas con la diferencia.

  - Visible en Tiendas: que el concepto sea visible en las tiendas.

  - Activo. si está en uso u obsoleto.

Desde la pantalla de Mantenimiento de Conceptos de Almacén para Venta se podrán listar todos los conceptos pulsando el botón **“Consultar”.**

![](/media/image216.png)

También será posible filtrar por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Concepto de Almacén para Venta:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono ![](/media/image19.png)

### Mantenimiento de Conceptos de Almacenes para Compras ![](/media/image217.png)

La posibilidad de automatizar determinados criterios que se produzcan al realizar un pedido de Compras.

En este punto de menú se darán de alta tantos conceptos como situaciones diferentes se produzcan en una operación de compras.

![](/media/image218.png)

![](/media/image219.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de hasta 4 dígitos.

  - Descripción: nombre del concepto.

  - Signo: Se permitirá seleccionar entre (+) Positivo, (-) Negativo o () Sin Signo.

  - Operación almacén: Vendrá condicionado por el signo seleccionado, tomando los valores: Entrada, Salida o No aplica.

  - Almacén destino: para predeterminar el almacén de destino.

  - Activo: si está en uso u obsoleto.

  - Aceptación Automática de Pedidos: si se chequea esta casilla el Pedido de Compra no contemplará el estado PENDIENTE DE ACEPTACIÓN. De forma que pasará directamente del estado SOLICITUD DE PEDIDO al estado EN PREPARACIÓN.

  - Generación Automática de Pedidos de Faltas: si se chequea esta casilla, para Pedidos de Compras, en el caso de que la cantidad pedida y la cantidad servida sean diferentes se generará automáticamente un pedido de faltas con la diferencia.

Desde la pantalla de Mantenimiento de Conceptos de Almacén para Compras se podrán listar todos los conceptos pulsando el botón “**Consultar”.**

![](/media/image220.png)

También será posible filtrar por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Concepto de Almacén para Compras:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Tipos de Contacto ![](/media/image221.gif)

Los tipos de contacto permiten establecer diferentes vías mediante las cuales se pueda mantener contacto con los clientes. Para realizar una búsqueda de los tipos de contacto se permite filtrar por código y descripción, además de poder buscarse los registros activos/inactivos.

![](/media/image222.png)

Los campos a rellenar para cada tipo de contacto son:

![](/media/image223.png)

  - Código: Alfanumérico, tiene que ser único para cada tipo de contacto.

  - Descripción: Breve descripción identificativa del tipo de contacto.

  - Buzón: Cada contacto se puede asociar con un buzón creado desde el mantenimiento de buzones.

  - Orden: Campo numérico para establecer un orden entre los diferentes tipos de contacto.

  - Protocolo: Protocolo correspondiente al tipo de contacto.

  - Visible: Se determina si el tipo de contacto está visible/oculto para el cliente.

  - Puede recibir notificaciones: Se marca si el tipo de contacto va a ser usado para hacer llegar notificaciones al cliente.

  - Activo: Permite definir cuando un tipo de contacto se encuentra activo/inactivo.

Desde el mantenimiento de tipos de contacto es posible realizar el Alta/Edición/Consulta y Baja de una tipo de contacto:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un tipo de contacto se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Consultar los Servicios

Desde este apartado se puede acceder a los servicios existentes para los diferentes almacenes a los que tiene acceso el usuario.

El primer paso para consultar los servicios es seleccionar el almacén del que se quiere hacer la consulta.

![](/media/image224.png)

Tras seleccionar el almacén, se muestra una pantalla de consulta que permite realizar la búsqueda de servicios filtrando por diferentes criterios:

  - ID Servicio: Permite buscar un servicio concreto mediante su identificador. Es posible realizar búsquedas por coincidencia de caracteres, utilizando el carácter ‘%’ tanto al principio como al final del campo.

  - Tipo Documento: Consta de dos campos de tipo ayuda. En el primero se define el país al que pertenece el documento, y en el segundo el tipo de documento, entre los existentes para el país seleccionado.

  - Cód. Documento Origen: Permite buscar un servicio a partir del código de su documento origen. Es posible realizar búsquedas por coincidencia de caracteres, utilizando el carácter ‘%’ tanto al principio como al final del campo.

  - Tipo de Servicio: Permite realizar la búsqueda filtrando por el tipo de servicio.

  - Almacén Origen: Campo de tipo ayuda para seleccionar el almacén de origen del servicio.

  - Almacén Preparación: Campo de tipo ayuda para seleccionar el almacén de preparación del servicio.

  - Almacén Destino: Campo de tipo ayuda para seleccionar el almacén de destino del servicio.

  - Fecha registro desde/hasta: Dos campos de tipo fecha que permiten establecer un rango para filtrar según la fecha en que se hizo el servicio.

  - Fecha solicitud desde/hasta: Dos campos de tipo fecha que permiten establecer un rango para filtrar según la fecha en que se solicitó la entrega del servicio.

  - Estados: Mediante selectores se permite buscar servicios que se encuentren en determinados estados.

![](/media/image225.png)

Pulsando sobre el Id Servicio en la rejilla de resultados, o sobre el icono![](/media/image18.png), se accede a la pantalla de detalle del servicio.

La pantalla de detalle de un servicio consta de 4 pestañas:

**Cabecera**

En esta pestaña se encuentran los datos genéricos del servicio, organizados en cajetillas:

  - Datos del Servicio: Se muestran la información del propio servicio.

  - Datos del Fidelizado: En el caso de que el servicio esté vinculado a un fidelizado, se muestran aquí los datos del mismo.

  - Contactos: Se muestra las diferentes vías de contacto con el receptor del servicio.

  - Observaciones: Campo de texto libre donde se pueden incluir observaciones relativas al contacto.

  - Importe e importe pendiente: Se muestra el importe total del servicio y el importe pendiente de pago.

  - Estado del servicio y fecha de estado: Se muestra el estado actual de servicio y la fecha en la que pasó a dicho estado.

![](/media/image226.png)

![](/media/image227.png)

**Servicios de preparación**

En esta pestaña se muestran las diferentes preparaciones asociadas al servicio. En una rejilla se muestran las rutas de preparación, así como los artículos que deben prepararse de cada ruta, los preparados, los pendientes de preparar, los que han sido sustituidos y los que no han sido servidos. En la misma tabla se muestran las fechas de inicio y de fin de la preparación, así como observaciones hechas por el preparador.

En otra rejilla se muestra un resumen de los bultos asociados al servicio, detallándose el tipo de embalaje de cada bulto, el contenido, el número total de bultos y el peso.

![](/media/image228.png)

**Solicitudes asociadas**

Desde esta pestaña se muestran todas las solicitudes asociadas al servicio. Además, para cada solicitud se muestra una rejilla con las actividades asociadas a la misma.

![](/media/image229.png)

**Histórico de estados**

Desde esta pestaña se accede a una rejilla que muestra todos los cambios de estado del servicio, mostrándose la fecha y el responsable de cada cambio de estado.

![](/media/image230.png)

### Subida manual de documentos ![](/media/image231.png)

El procesamiento de documentos de forma manual está orientado a casos en que no sea posible tramitar los tickets de manera automática debido a problemas de conexión. Mediante esta opción se posibilita la subida de ficheros que previamente hayan sido descargados desde el InStoreEngine de comerzzia para su procesado. Los ficheros a procesar son archivos xml que contienen la información y configuración necesaria para la generación de un servicio.

![](/media/image232.png)

## Configuración de Terceros (Clientes-Proveedores)

### Mantenimiento de Sectores ![](/media/image233.png)

Los sectores se identifican como un criterio para realizar agrupaciones de Clientes.

En este punto de menú se darán de alta los diferentes sectores para posteriormente poder asociar en el cliente el sector al que pertenece.

![](/media/image234.png)

Los campos de la pantalla son los siguientes:

  - Código: puede ser alfanumérico de 4 dígitos

  - Descripción: Nombre del sector

  - Activo: identifica si el registro está activo u obsoleto.

Desde la pantalla de Mantenimiento de Sectores se podrán listar todos los conceptos pulsando el botón **Consultar.**

![](/media/image235.png)

También será posible filtrar por el código o la descripción.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Sector:

  - Alta/Edición/Consulta/Baja de Sectores

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Clientes ![](/media/image236.png)

La posibilidad de dar de alta todos los clientes con los que trabaje la empresa asociándoles una serie de características que posteriormente se recuperen automáticamente en los procesos de venta.

En este punto de menú se darán de alta los clientes con los que se realicen operaciones de pedidos, albaranes o facturas de venta.

Aunque para el alta sólo serán obligatorios los campos código, descripción y Tratamiento de Impuestos, se recomienda rellenar todos los campos posibles para recuperarlos automáticamente en los procesos relacionados con clientes.

La pantalla se compone de dos bloques:

En un primer bloque aparecen los **datos del Cliente**:

![](/media/image237.png)

  - Código: puede ser alfanumérico de hasta 11 dígitos

  - Descripción: Nombre del cliente

  - Activo: si se puede usar

El segundo Bloque contiene tres pestañas o botones de enlace, visualizándose información distinta según en la pestaña que se posicione el usuario:

![](/media/image238.png)

  - **Pestaña Datos Generales:**

![](/media/image239.png)

> **<span class="underline">Contacto:</span>**

Aparecen los datos Nombre comercial de la empresa, persona de contacto, domicilio, población, provincia, código postal, país, teléfonos, fax, e-mail.

> **<span class="underline">Datos fiscales: </span>**

  - Tipo de documento identificativo y número de documento identificativo asociado al cliente.

  - Tratamiento de impuestos: campo de ayuda donde debe seleccionarse el tipo de impuesto que le corresponde al cliente (Nacional, Exportación/Importación, Intracomunitario, IGIC, etc.). Es muy importante realizar bien esta selección, ya que el tipo de impuesto asociado al cliente será uno de los datos que se tendrá en cuenta para calcular los impuestos en los procesos de ventas. Los diferentes impuestos aplicables se deberán haber dado de alta previamente en el Mantenimiento de Tratamiento de Impuestos (punto 2.9 de este manual)

  - Medio de pago: campo ayuda que recuperará las formas de pago que se hayan dado de alta en el Mantenimiento de Medios de Pago (efectivo, tarjeta, cheque, transferencia, pagaré, giro, etc.). (punto 2.15 de este manual)

  - Tarifa: campo ayuda que permitirá asociar una tarifa al cliente para que se aplique directamente al realizar los documentos de venta (pedidos, albaranes y facturas). Previamente tendrán que haber sido dadas de alta las tarifas en el Mantenimiento de Tarifas. (para más detalle consultar el Mantenimiento de Tarifas).

  - Riesgo concedido: Importe de riesgo concedido al cliente.

> **<span class="underline">Organización: </span>**

  - Sector: campo ayuda que recuperará los sectores que se hayan dado de alta en el Mantenimiento de sectores.

<!-- end list -->

  - **Pestaña de Datos Bancarios: **

![](/media/image240.png)

  - Nombre del banco, domicilio, población y CCC. El CCC que se inserte en este punto de menú se utilizará posteriormente en procesos de Tesorería como son las Remesas Bancarias.

<!-- end list -->

  - **Pestaña de Observaciones:**

![](/media/image241.png)

  - Campo texto donde se podrán hacer anotaciones o insertar otra información relevante acerca del cliente.

Desde la pantalla de Mantenimiento de Clientes se podrán listar todos los conceptos pulsando el botón **Consultar.**

![](/media/image242.png)

También será posible filtrar por el código o la descripción, Nombre Comercial o CIF.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Cliente:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

### Mantenimiento de Tarifas

Desde el mantenimiento de tarifas se permite gestionar las diferentes tarifas con las que se cuenta. Es posible realizar el Alta/Edición/Consulta y Baja de una tarifa:

  - Para dar de alta una tarifa hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

![](/media/image243.png)

Para la creación de una tarifa se debe definir:

  - Código: Código identificativo único de la tarifa.

  - Descripción: Título descriptivo de la tarifa.

  - Versión:

  - País: País en que aplica la tarifa.

  - Tratamiento impuestos: Campo que tira del mantenimiento de tratamiento de impuestos.

Búsqueda de artículos: Se permite buscar los artículos que forman parte de la tarifa, filtrando por, descripción, familia y proveedor.

![](/media/image244.png)

Desde el modo edición, se permite añadir artículos a la tarifa, eliminarlos, o editar los registros.

![](/media/image245.png)

### Mantenimiento de Promociones

El mantenimiento de promociones está detallado en el manual de promociones “COM\_USR\_MANUAL DE GESTIÓN DE PROMOCIONES”.

### Mantenimiento de Canales de Venta

Desde este mantenimiento se pueden definir los diferentes canales de venta que se asignarán a las tiendas. Los canales de venta agrupan los diferentes productos y artículos que se comercializan.

![](/media/image246.png)

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un canal de venta:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

Para definir un canal de venta se requiere:

  - Código: Identificador único para cada canal de venta

  - Descripción: Título descriptivo del canal de venta

![](/media/image247.png)

  - En la pestaña Datos Generales, se debe determinar las tarifas asociadas al canal de venta.

  - Descripción: Nombre del canal de venta.
    
      - Tarifa: Tarifa asociada al Canal de venta. Las tarifas asociadas a un canal de venta deberán haber sido dadas de alta desde el mantenimiento de tarifas. La que quede vinculada al canal de venta mediante el campo Tarifa será la que aplique en la tienda virtual.
    
      - Tarifa de referencia: Sirve para comparar los precios de los artículos con los de la tarifa vinculada mediante el campo Tarifa, cuyos importes serán los definitivos. En la versión 4.0 de comerzzia no aplica la tarifa de referencia.

  - En la pestaña Productos se añaden uno a uno todos los productos que forman parte del canal de venta.

  - En la pestaña Artículos se añaden uno a uno todos los artículos que forman parte del canal de venta.

> ![app-bg-tooltip](/media/image248.png) Para la configuración de tiendas desde el Mantenimiento de Tiendas, es necesario asignar a cada tienda un Canal de Venta que defina el surtido de productos y artículos que vende.

### Mantenimiento de Proveedores ![](/media/image249.png)

Desde la pantalla de Mantenimiento de Proveedores se podrán gestionar todos los proveedores pulsando el botón **Consultar.**

![](/media/image250.png)

También será posible filtrar por el código, la descripción o el CIF.

Desde aquí será posible realizar el Alta/Edición/Consulta y Baja de un Proveedor:

  - Para dar de alta un registro hay que posicionarse sobre el botón ![](/media/image16.png) Añadir de la cabecera.

  - Para Editar un registro se utilizará el icono ![](/media/image17.png) de la barra de acciones.

  - Para consultar un registro en concreto se puede hacer con un ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

Desde la opción ![](/media/image16.png) Añadir se darán de alta los proveedores con los que se realicen operaciones de albaranes o facturas de compras.

La pantalla se encuentra dividida en dos bloques:

![](/media/image251.png)

Aunque los únicos datos obligatorios son el código, la descripción y el Tratamiento de Impuestos se recomienda que se rellenen todos los datos posibles para que posteriormente se automaticen en los procesos de compras.

En el primer bloque se identificarán los **datos del proveedor**:

![](/media/image252.png)

  - Código: puede ser alfanumérico de hasta 11 dígitos.

  - Descripción: Nombre del Proveedor

  - Activo: si está en uso.

En el segundo bloque aparecen 3 pestañas, Datos Generales, Datos Bancarios y Observaciones, visualizándose información diferente en función de la pestaña en que se posicione:

  - **Pestaña Datos Generales:**

![](/media/image253.png)

**<span class="underline">Contacto:</span>** se identifican el nombre comercial del proveedor (que podría ser diferente o no a la Descripción), nombre de la persona de contacto, domicilio, población, provincia, país, código postal, teléfono, fax y email.

**<span class="underline">Datos fiscales,</span>** aparecen los siguientes datos:

  - Tipo de documento identificativo y número de documento: se debe rellenar el número de documento identificativo de la empresa, que será necesario para poder facturar. Al Crear por primera vez el registro o al editar ![](/media/image17.png) aparecerá a la derecha del campo el icono ![](/media/image254.png) que permite validar el CIF.

  - Tratamiento de Impuestos: campo ayuda que recuperará los valores dados de alta en el Mantenimiento de Impuestos. El tratamiento de Impuestos asociado al proveedor (Nacional, Importación/Exportación, Intracomunitario, etc.) es muy importante, ya que será uno de los criterios por los que se calculen los impuestos en los procesos de compras.

  - Modo de Pago: campo ayuda que recupera los valores dados de alta en el Mantenimiento de Medios de Pago. Al asociar una forma de pago al proveedor se permite que posteriormente se recupere automáticamente en los procesos de compra.

**<span class="underline">Organización:</span>** se identificará el **tipo de Proveedor** identificando si es Proveedor, Fabricante o Acreedor.

  - **Pestaña Datos Bancarios:**

![](/media/image255.png)

Se identificará el nombre del banco que se utilice para los pagos del proveedor, insertando los datos de domicilio, población y CCC.

  - **Pestaña Observaciones:**

![](/media/image256.png)

Campo texto donde se podrán hacer anotaciones o insertar otra información relevante acerca del proveedor.

## Configuración de Canales y Buzones

### Mantenimiento de Buzones ![](/media/image257.png)

El mantenimiento de buzones en comerzzia permite acceder a los diferentes buzones definidos para la organización. Para consultar los diferentes registros se puede filtrar por código y por descripción.

![](/media/image258.png)

Las funcionalidades del mantenimiento de buzones son:

  - Dar de alta un nuevo buzón, pulsando sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar un buzón utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar un buzón en concreto haciendo ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Para dar de baja un registro se utilizará el icono![](/media/image19.png).

En el alta de un nuevo buzón son obligatorios:

  - El número de buzón, que se emplea como código y por tanto debe ser único para cada buzón.

  - La descripción, que sirve para identificar al buzón.

  - La prioridad que se le asigna al buzón.

Otros campos complementarios a rellenar son la plantilla del buzón, destinatario, URL de confirmación de lectura, y los días en que se guardan los históricos antes de eliminarse los mensajes, además de los canales que se emplean para el buzón.

![](/media/image259.png)

![](/media/image260.png)

### Mantenimiento de Plantilla de Buzones ![](/media/image261.png)

El mantenimiento de plantilla de buzones es un mantenimiento simple de comerzzia orientado a dar soporte al mantenimiento de buzones.

La consulta de las plantillas se puede filtrar por código y por descripción.

![](/media/image262.png)

Las funcionalidades del mantenimiento de plantillas de buzones son:

  - Dar de alta una nueva plantilla de buzones, pulsando sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar una plantilla de buzones utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar una plantilla de buzones haciendo ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

  - Dar de baja un registro utilizando el icono![](/media/image19.png).

La información a cumplimentar para dar de alta una nueva plantilla es:

  - Código: identificador único para cada plantilla.

  - Descripción: título identificativo de la plantilla.

  - Plantilla: nombre del archivo que contiene la plantilla velocity que se desea importar.

### Mantenimiento de Canales ![C:\\Users\\tier1\\AppData\\Local\\Microsoft\\Windows\\INetCache\\Content.Word\\canales.gif](/media/image263.gif)

Desde el mantenimiento de canales se pueden configurar los diferentes canales de comunicación de la organización. La búsqueda para de canales se puede filtrar por código y descripción.

![](/media/image264.png)

Las funcionalidades del mantenimiento de canales son:

  - Dar de alta un nuevo canal, pulsando sobre el botón ![](/media/image16.png)Añadir de la cabecera.

  - Editar un canal de comunicación existente utilizando el icono ![](/media/image17.png) de la barra de acciones.

  - Consultar un canal existente haciendo ‘click’ de ratón sobre el campo código o con el icono ![](/media/image18.png)

Para definir un canal de comunicación se requiere la siguiente información:

  - Código: Identificador único para cada canal.

  - Descripción: Título descriptivo del canal.

  - Tipo de canal: Pueden ser de salida, de entrada o de procesamiento

  - Clase control.

  - Ámbito aplicación: Campo que sirve para esclarecer cuando se va a usar el canal.

  - Último error.

  - Parámetros del canal: Se pueden definir los parámetros del canal y el valor de los mismos. Se deben configurar los parámetros:
    
      - SMTP\_USUARIO y SMTP\_CLAVE: Credenciales de acceso al servidor de correo. Puede no ser necesario, dependiendo del propio servidor.
    
      - SMTP\_HOST: Host del servidor de correo.
    
      - SMTP\_PUERTO: Puerto del servidor de correo.
    
      - SMTP\_ORIGEN\_NOMBRE: Nombre que aparecerá como remitente en los correos.
    
      - SMTP\_ORIGEN\_EMAIL: Email que aparecerá como remitente en los correos

![](/media/image265.png)

# SINCRONIZACIÓN CENTRAL - TIENDAS

El proceso de sincronización tiene como objetivo, dependiendo del tipo de tienda, preparar o enviar a las tiendas los datos que necesitan para su funcionamiento y, a su vez, recibir los que éstas generan.

##  Métodos de sincronización

Comerzzia permite sincronizar la información desde central a tiendas y desde tiendas a central utilizando los siguientes métodos:

  - **Conexión Online.** No es necesaria sincronización porque las tiendas acceden directamente a la base de datos de la oficina central por estar siempre online.

  - **Conexión Offline con sincronización Centralizada.** La tienda tiene su propia Base de datos. La actualización se realiza desde el servidor central que accede directamente a la base de datos de la tienda para actualizar o leer sus datos.

  - **Conexión Offline con sincronización Remota.** La tienda tiene su propia Base de datos. La actualización se realiza desde la tienda desde el módulo in-store engine, que es el encargado se solicitar y enviar datos vía webservice a la central.

  - **Conexión Offline con sincronización Remota y POS autónomo**. Igual que el caso anterior, pero se instala una base de datos por cada POS.

### Sincronización Offline Centralizada

Existe un planificador de tareas en el servidor central para que estas se ejecuten cada cierto tiempo configurable de manera periódica. Existen diferentes tareas para cada tienda. La ejecución de una tarea, abre una conexión con la base de datos de la tienda que corresponda y actualiza sus tablas o lee los registros necesarios para copiarlos en la central.

  - Requisitos: Se requiere visibilidad IP desde la central a cada una de las tiendas. El puerto de la base de datos de cada una de las tiendas debe de estar abierto para que desde la central se pueda conectar a la base de datos de la tienda.

  - Ventajas: El proceso está centralizado y se puede controlar todo desde la central. No requiere instalar módulo de sincronización *in-store engine* en las tiendas.

  - Inconvenientes: No permite configurar conexión SSL. Se requiere visibilidad IP a cada una de las tiendas y que estas mantengan IP fija. Se requiere que el puerto de las bases de datos de cada tienda esté abierto para acceso desde servidor central.

### Sincronización Offline Remota

Descripción: Existe un planificador de tareas en el módulo in-store engine instalado en cada tienda. Estas tareas se ejecutan cada cierto tiempo configurable de manera periódica. La ejecución de una tarea realiza una petición a un webservice de la central vía HTTP enviando datos o solicitando actualizaciones.

  - Requisitos: Se requiere visibilidad IP desde cada tienda a la central para realizar una petición HTTP o HTTPS. Se requiere instalar módulo de sincronización in-store engine en cada tienda.

  - Ventajas: Permite configurar conexión SSL. No requiere IP fijas en las tiendas. Las operaciones se realizan vía webservice sin acceso remoto directo a las bases de datos. La carga de sincronización se encuentra distribuida haciendo más ligero el servidor central.

  - Inconvenientes: Existe un menor control de supervisión por parte del usuario del proceso de sincronización. Al no estar centralizado en un único sitio, se requiere que los módulo in-store engine de cada tienda estén arrancados y funcionando para asegurar que los datos se están actualizando.

### Sincronización Offline Remota con POS Autónomo

Descripción: La arquitectura es idéntica al caso anterior, con la salvedad de que se instala una base de datos y un módulo in-store engine en cada terminal POS de la tienda.

  - Requisitos: Se requiere visibilidad IP desde cada POS de la tienda a la central para realizar una petición HTTP o HTTPS. Se requiere instalar módulo de sincronización in-store engine en cada POS de la tienda.

  - Ventajas: Igual que en el caso anterior. Además:
    
      - El POS puede funcionar de manera autónoma aunque la red de la tienda deje de funcionar momentáneamente.
    
      - Como cada POS tiene su propia base de datos, no requieren conectarse a un POS Máster, pudiendo funcionar todos de manera autónoma.

  - Inconvenientes: Igual que en el caso anterior. Además:

  - Determinadas operaciones no pueden realizarse de manera común en toda la tienda, ya que los datos no son compartidos al existir una base de datos independiente por POS. En general, cualquier operación sobre base de datos desde el POS será invisible para el resto de POS. Por ejemplo:
    
      - Si se registra un cliente en un POS sólo se hace en la base de datos de ese POS.
    
      - Los POS no pueden consultar los tickets realizados en otro POS.
    
      - El cambio de permisos de usuario debe hacerse en cada POS.
    
      - El cambio de password de cada usuario debe hacerse en cada POS o desde backoffice.

  - El proceso de sincronización es más lento y costoso debido a que existen muchas más bases de datos que actualizar.

# ADMINISTRAR Y MONITORIZAR EL SISTEMA EN LA CENTRAL

## Administración del Sistema/Sincronizador/Procesador de Datos

El punto “Administrador del Sistema” consta de tres pestañas, tal y como se puede ver en la imagen que sigue:

![](/media/image269.png)

La primera de ellas muestra el estado del Sincronizador de Tiendas que podrá ser arrancado mediante el botón![](/media/image270.png). Una vez arrancado el sincronizador será posible detenerlo o reiniciarlo mediante los botones![](/media/image271.png).

![](/media/image272.png)

La segunda de las pestañas de este punto de menú es similar a la primera, pero aplicada al Procesador de Datos.

![](/media/image273.png)

La tercera pestaña muestra la configuración del sistema.

![](/media/image274.png)

Como se puede ver en la imagen, se distinguen tres bloques cuyas propiedades pueden ser modificadas una vez se haya editado la pantalla:

1.  Sincronizador de Tiendas: en él se pueden ver las siguientes propiedades a configurar:

<!-- end list -->

  - Arranque automático del sincronizador de tiendas: el sincronizador de tiendas se arrancará o no una vez que se arranque el servidor.

  - Número máximo de trabajos simultáneos que puede ejecutar el sincronizador.

  - Vista por defecto al entrar en la pantalla del sincronizador de tiendas.

  - Número de días que se mantendrán en base de datos las actualizaciones aplicadas y anuladas: permite indicar el número de días que se mantendrán en el servidor los ficheros de actualización de tiendas aplicados y anulados, antes de que sean borrados.

<!-- end list -->

2.  Tickets:

<!-- end list -->

  - Activación automática del servicio de procesamiento de datos.

  - Tiempo en segundos de demora entre procesamientos.

<!-- end list -->

3.  Conexión:

<!-- end list -->

  - Ruta del WebService de clientes.

  - Ruta del WebService de sincronización.

  - Ruta del WebService de usuarios.

  - Ruta del WebService de servicios REST.

## Estadísticas de uso

Este punto de menú muestra el XML de Estadísticas. Es posible exportarlo mediante el botón![](/media/image275.png).

![](/media/image276.png)

## Bus de Integración (ESB)

Comerzzia 3.x tiene una arquitectura SOA que es soportada a través del BUS de Integración (ESB). El ESB es el encargado de establecer la comunicación entre el POS Máster, los servicios centrales y dispositivos adicionales en tienda (FastPOS, Balanzas, etc.). Adicionalmente, está preparado para implementar los mecanismos de integración con organismos públicos, empresas de transporte, notificaciones al cliente final, etc..

Otra de las funcionalidades que aportará es la separación de ciertos servicios que actualmente implementa únicamente el POS, como los de impresión, pasarela de pago, promociones, fidelización, etc... Esto permitirá a las diferentes aplicaciones de venta multi-canal acceder a estos servicios directamente (por ejemplo, FastPOS, CheckPricer, WebKiosk, etc.)

Desde este punto de menú se gestiona el estado de funcionamiento del ESB:

![](/media/image278.png)

Desde este menú se podrá:

  - Arrancar el ESB mediante el botón![](/media/image270.png).

  - Detener o Reiniciar el ESB mediante los botones![](/media/image271.png).

## Eventos ![](/media/image279.gif)

Desde este apartado se puede consultar un registro de eventos que hayan sido definidos. En el estándar se registran los accesos a la plataforma de backoffice de comerzzia. Se permite consultar los registros filtrando por fecha, usuario, componente, acción y severidad del evento.

![](/media/image280.png)

# MONITORIZACIÓN DEL SINCRONIZADOR DE TIENDAS

Para poder ejecutar el proceso de sincronización es necesario que el “Sincronizador de Tiendas” esté en funcionamiento.

La supervisión de todos los trabajos de sincronización con las Tiendas se realiza desde el menú **“Almacén-Tienda”-\>Sincronizador de Tiendas. **

En caso de que al acceder a este elemento de menú aparezca el siguiente mensaje, será necesario arrancar los servicios de Sincronización y procesado de documentos desde el menú de **“Sistema”**:

![](/media/image281.png)

El monitor nos ofrece la relación de trabajos de sincronización, en tres vistas alternativas:

  - **Vista Trabajos por Tipos:** Muestra los trabajos de sincronización agrupados por Tipo de Trabajos

  - **Vista Trabajos por Tiendas:** Muestra los trabajos de sincronización agrupados por cada Tienda.

  - **Vista Actualizaciones:** Listado de todas las actualizaciones generadas para todas las tiendas, mostrando de forma resumida los datos asociados a cada una de ellas.

  - **Vista Consulta de Trabajos:** Permite realizar una consulta selectiva de los trabajos de actualización en función de los criterios seleccionados por el usuario.

## Trabajos disponibles según tipo de sincronización de Tienda

En función del tipo de sincronización de cada tienda, estarán disponibles el siguiente conjunto de trabajos de sincronización:

1.  **Tienda con sincronización ON-LINE:** No tiene asociada trabajos de sincronización puesto que la tienda comparte la base de datos de la Central.

2.  **Tienda con sincronización OFF-LINE Centralizada:** En este tipo de sincronización, la central conoce la ubicación de la base de datos de la tienda, por lo que, cuando se ejecuten los trabajos indicados a continuación, los datos asociados serán almacenados o consultados directamente en la base de datos de la tienda. En este caso existen 4 trabajos de sincronización, indicados a continuación:
    
    1.  Enviar Configuración.
    
    2.  Enviar Artículos.
    
    3.  Recibir Cierres de Caja.
    
    4.  Recibir Documentos.

3.  **Tienda con sincronización OFF-LINE Remota:** En este tipo de sincronización, la central desconoce la ubicación de la base de datos de la tienda, por lo que, cuando se ejecuten los trabajos indicados a continuación, los datos asociados serán depositados en un paquete de actualización en la propia central, que será consultado por la tienda cuando se conecte a la misma de forma remota para consultar las actualizaciones asociadas a la misma. En este caso, existen 2 trabajos de sincronización, indicados a continuación:
    
    5.  Generar Datos Configuración.
    
    6.  Generar Actualización Artículos.

## Trabajos de Sincronización Central - Tiendas

A continuación se detallan los tipos de trabajos de sincronización mencionados anteriormente.

### Trabajo “Enviar Configuración”

Envía o prepara todos los datos de configuración de la tienda, tanto para una tienda que está funcionando, actualizando posibles cambios, como para una tienda “desde cero” que necesita ser “inicializada”.

Este trabajo siempre es forzado. En caso de que se envíe el fichero de configuración a tiendas ya existentes, se actualizará la configuración del POS así como se crearán nuevas variables en el fichero de configuración del POS, si procede.

Los datos de configuración referenciados son:

  - Usuarios (de la tienda) y Perfiles

  - Variables

  - Impuestos

  - Medios de Pago

  - Cajas

  - Información propia de la Tienda.

### Trabajo “Enviar Artículos”

Envía o prepara todos los datos relacionados con los Artículos:

  - Categorización de los Artículos

  - Artículos

  - Tarifas y Promociones

Los Artículos y Tarifas/Promociones se procesan sujetos a **versiones**, de forma que el sistema gestiona internamente diferencias de información entre Central y Tiendas, a efectos de sincronización de datos.

### Trabajo “Recibir Documentos”

Recepción de los documentos de venta generados en las tiendas. Sólo se reciben, no se procesan en este “trabajo”. Estarán disponibles para su monitorización desde el menú **“Procesamiento de Documentos”.**

### Trabajo “Recibir Cierres de Caja”

Recepción de los cierres de las cajas generados en las tiendas. Este trabajo sólo se encarga de recibir los cierres y almacenarlos en el sistema, para su posterior procesado monitorizable desde el menú **“Procesamiento de Documentos”,** ya que los cierres de caja serán tratados por el sistema como un tipo de documento más.

### Trabajo “Generar Actualización de Artículos”

Genera los datos de actualización de artículos que posteriormente serán sincronizados por el sincronizador remoto.

### Trabajo “Generar Datos Configuración”

Genera los datos de configuración que posteriormente serán sincronizados por el sincronizador remoto.

## Detalle de cada Interfaz disponible en el Sincronizador de Tiendas

En las interfaces descritas a continuación, se visualiza el listado de trabajos de sincronización organizado por diferentes criterios. Para cada trabajo, se podrá visualizar la siguiente información (campos) en pantalla:

  - Trabajo: nombre del Trabajo listado.

  - Tienda: código de la tienda asociada al Trabajo de sincronización.

  - Descripción: Nombre descriptivo asociado a la tienda.

  - Estado:

> ![](/media/image282.png) Arrancado
> 
> ![](/media/image283.png) Parado
> 
> ![](/media/image284.png) Pausado

  - Fecha de Inicio: Cuándo se arrancó el trabajo.

  - Fecha de Próxima Ejecución: según programación (“ejecutar periódicamente”) o indicada manualmente en la edición del Trabajo.

![](/media/image285.png)

  - Intervalo: según programación (“ejecutar periódicamente”).

  - Fecha de Última Ejecución: Cuándo se ejecutó por última vez.

  - Resultado:

> ![](/media/image286.png) Trabajo realizado correctamente.
> 
> ![](/media/image287.png) El Trabajo no se ha podido realizar / Trabajo con errores.

A continuación se detallan las diferentes vistas disponibles desde el Menú.

### Listado de Trabajos de Sincronización: Vista Trabajos por Tipo

El monitor nos ofrece la relación de trabajos de sincronización, agrupados, en esta vista, por tipologías de trabajos:

  - Tipo Trabajo “Enviar Artículos”:

![](/media/image288.png)

  - Tipo Trabajo “Enviar Configuración”:

![](/media/image289.png)

  - Tipo Trabajo “Generar Actualización de Artículos”

![](/media/image290.png)

  - Tipo Trabajo “Generar Datos de Configuración”

![](/media/image291.png)

  - Tipo Trabajo “Recibir Cierres de Cajas”

![](/media/image292.png)

  - Tipo Trabajo “Recibir Documentos”

![](/media/image293.png)

### Listado de Trabajos de Sincronización: Vista Trabajos por Tiendas

El monitor nos ofrece la relación de trabajos de sincronización, agrupados, en esta vista, por Tiendas:

![](/media/image294.png)

### Listado de Trabajos de Sincronización: Vista Actualizaciones

Existe la posibilidad de consultar todas las actualizaciones generadas para todas las tiendas, conociendo el estado de dicha actualización, así como poder descargar el fichero xml que corresponde a la actualización. Se pueden filtrar los resultados obtenidos indicando la tienda y las fechas para las que queremos obtener las actualizaciones en el panel de búsqueda.

![](/media/image295.png)

El listado ofrece la siguiente información para cada actualización generada:

  - Tienda: Código de almacén asociado a la tienda

  - Descripción: Descripción de la tienda

  - ID: Identificador único asociado al paquete de actualización.

  - Tipo: Tipo de actualización (artículos o configuración)

  - Fecha Generación: Fecha en la que se generó la actualización

  - Fecha Transmisión: Fecha en la que la actualización ha sido transmitida. Si no muestra información, es que la actualización está pendiente de ser transmitida.

  - Fecha Aplicación: Fecha en la que la actualización ha sido aplicada en la tienda. Si no existe, es que la actualización todavía no ha sido aplicada.

  - Estado: Resultado de la aplicación de la actualización. Sus posibles valores son:

> ![](/media/image296.png) Pendiente
> 
> ![](/media/image297.png) Aplicada
> 
> ![](/media/image298.png) Errónea

  - Forzada: Muestra información sobre si la actualización ha sido forzada de forma manual a través del botón de ejecución inmediata ![](/media/image299.png) o no.

  - Acciones: Ofrece al usuario un conjunto de acciones disponibles sobre la actualización:
    
      - ![](/media/image300.png) : la posibilidad de obtener el fichero correspondiente a la actualización en formato XML. Para descargar el fichero, pulsar sobre el icono ![](/media/image300.png).
    
      - ![](/media/image301.png): eliminar la actualización seleccionada.
    
      - ![](/media/image302.png): Anula la actualización seleccionada.

### Listado de Trabajos de Sincronización: Consulta de Trabajos

En esta pestaña se puede ver un formulario de consulta en la línea del resto de pantallas de consulta de la aplicación.

![](/media/image303.png)

Se mostrarán todos los trabajos existentes en función de los filtros introducidos en el bloque de búsqueda, pudiéndose actualizar los resultados de dicha búsqueda. Los filtros mencionados son los siguientes:

  - Tienda (desde - hasta), obtenidas mediante la ayuda correspondiente.

  - Agrupado, muestra los valores definidos para este campo mediante un desplegable.

  - Tipo de Trabajo.

  - Estado.

  - Trabajo con Errores, filtro que hará que se muestren o no aquellos trabajos que han presentado o no, errores en su ejecución, respectivamente.

Para poder visualizar los resultados en modo ficha, bastará con hacer click sobre el botón ![](/media/image304.png). Si además se pretende planificar la ejecución de dicho trabajo se pulsará sobre el botón ![](/media/image305.png).

La pantalla de detalle de un trabajo es la siguiente:

![](/media/image306.png)

En caso de editar dicha pantalla, se mostrará la fecha y la hora de la próxima ejecución del trabajo en cuestión.

## Mantenimiento de los Trabajos de Sincronización

El administrador de comerzzia puede llevar a cabo el mantenimiento de los trabajos de sincronización de la forma comentada a continuación.

A través del Listado de Trabajos de Sincronización se puede acceder a cada uno de ellos para consultar ![](/media/image307.png) o planificar su ejecución![](/media/image305.png), así como para ejecutar acciones específicas de arranque![](/media/image308.png)/parada![](/media/image309.png)/pausa![](/media/image310.png).

![](/media/image311.png)Asimismo, es posible planificar![](/media/image312.png), arrancar![](/media/image313.png), pausar ![](/media/image314.png) y detener ![](/media/image315.png) varios trabajos simultáneamente seleccionándolos mediante los checks de cada uno de ellos![](/media/image316.png). También es posible seleccionar/deseleccionar todos los trabajos mediante la opción disponible en “Mas Acciones”:

También es posible realizar la ejecución forzada de un trabajo en el momento mediante la opción ![](/media/image299.png) “Ejecutar Ahora”.

### Programación de ejecución de trabajos: “Ejecutar periódicamente”

Los trabajos de sincronización permiten realizar una programación de la frecuencia de ejecución, lo que nos permite garantizar la integridad de la información en las tiendas con el periodo de tiempo que establezcamos.

La siguiente pantalla se muestra cuando se trata de planificar la ejecución de un trabajo, pulsando sobre el botón![](/media/image312.png):

![](/media/image317.png)

##  Procesamiento de Documentos

Para poder ejecutar el procesado de documentos es necesario que el “Procesador de Datos” esté en funcionamiento.

La supervisión de todos los trabajos de procesado de documentos provenientes de las Tiendas se realiza desde el menú **“Almacén-Tienda”-\>Procesamiento de Documentos. **

En caso de que al acceder a este elemento de menú aparezca el siguiente mensaje, será necesario arrancar los servicios de “Sincronizador y/o Procesador de Datos” desde el menú de **“Sistema”**:

![](/media/image318.png)

### Qué supone el procesado de Documentos en comerzzia

El procesado de documentos en comerzzia 3.x supone un concepto más amplio que un simple documento de venta.

Es por ello que existe el concepto **“Tipo de Documento”** mediante el que se identificará el tipo de documento procesado. Como tipo de documento estarán:

  - > Los **documentos de venta** parametrizados y que sea posible generar desde cada tienda, en función de su país de pertenencia. En la actualidad, se procesan las facturas simplificadas, facturas completas, notas de crédito así como los tipos de documentos de venta específicos de los países contemplados en la internacionalización de comerzzia. Para más información, consultar los manuales de Internacionalización por países. Los diferentes tipos de documentos de venta disponibles en comerzzia 3.0 son:
    
      - > Ventas por cliente: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por cliente.
    
      - > Ventas por familias: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por familia.
    
      - > Ventas por artículos: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por artículo.
    
      - > Ventas por tiendas: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por tienda.
    
      - > Ventas por franja horaria: Muestra todas las ventas que cumplen los parámetros indicados, agrupando por franja horaria del día.

  - Los cierres de caja, que quedan englobados en este concepto. Los **informes de cierres de caja** disponibles en comerzzia son:
    
      - > Cierre de caja totalizado: Muestra todos los cierres de caja que se han hecho por cada día, tienda y caja. En cada uno de ellos indica el total teórico, el total contado, y el descuadre entre ambos.
    
      - > Cierre de caja detallado: Muestra lo mismo que el anterior, pero desglosado por cada forma de pago.
    
      - > Movimientos de caja totalizados: Muestra, en el rango de fechas indicado, por cada tienda y caja, todos los apuntes de caja manuales (salida de efectivo, retirada de caja, etc.) agrupados por concepto.
    
      - > Movimientos de caja detallados: Muestra lo mismo que el anterior, pero desglosado por cada día dentro del rango de fechas seleccionado.
    
      - > Cierre de caja diferencia ventas: Muestra, en el rango de fechas indicado, por cada tienda, el total de ventas y el total teórico del cierre, así como su diferencia. Este cuadre debería ser siempre exacto, de lo contrario se trataría de un error de software (no humano).
    
      - > Desglose de ventas detallado: Muestra un desglose de las ventas para cada tienda y día según diferentes conceptos:
        
          - Ventas por caja
        
          - Ventas por vendedor
        
          - Ventas por forma de pago
        
          - Ventas por sección
        
          - Resumen cierre de caja
    
      - > Cierre de caja por turnos: Se considera un turno el periodo desde la apertura hasta el cierre de una caja. El informe de cierre de caja por turnos muestra un resumen de las ventas en cada uno de los turnos de las diferentes cajas.

  - Este concepto es ampliable a futuro a **otros tipos de documentos** que sea necesario procesar por el sistema, no necesariamente asociados a la venta.

El procesado de un documento supone el alta/inserción en el sistema de dicho documento, quedando asociado a:

  - La Serie de la Tienda que lo ha generado.

  - El Almacén asociado a la tienda que lo ha generado.

  - El Cliente con el que se realizó la venta (genérico de la tienda o específico)
    
      - El documento de venta hace referencia al Cliente a través del tipo de documento y número de identificación asociado. Si en el sistema no existe Cliente con el nº identificativo indicado en el ticket, la aplicación dará de alta, de forma automática, un nuevo Cliente con tipo de documento y código igual al especificado en el documento de venta.

  - El Concepto de Almacén de Venta será el Concepto especificado para la Tienda.

### Listado de Documentos pendientes de procesar

Presenta los documentos pendientes de procesar, agrupados por fecha y tienda

![](/media/image319.png)

### Listado de Tickets Procesados

Presenta los documentos procesados, agrupados por fecha y tienda, permitiendo establecer criterio de búsqueda por rango de fechas y Tienda:

![](/media/image320.png)

### Listado de Documentos Erróneos

Presenta los documentos con errores en el procesado, agrupados por fecha y tienda, permitiendo establecer criterio de búsqueda por rango de fechas y Tienda, e informando de la fecha del proceso y tipo de problema

![](/media/image321.png)

![](/media/image322.png)

Sobre esta pantalla podemos realizar las siguientes acciones:

![](/media/image323.png): Consultar y Editar el documento seleccionado

![](/media/image324.png): Borrar el documento seleccionado

![](/media/image325.png): Volver a procesar el documento seleccionado

![](/media/image326.png): Volver a procesar todos los documentos.

##  Actualización remota de Tiendas

Esta opción está disponible desde la V.3.0.3 desde el menú **“Almacén-Tienda”-\>Actualización de Tiendas.**

Al igual que se generan actualizaciones de configuración y artículos, desde esta opción de menú se pueden enviar actualizaciones que permitan enviar a las tiendas scripts de base de datos para que sean ejecutados en remoto. Las actualizaciones enviadas estarán disponibles para su consulta desde el menú **“Almacén-Tienda-\>Sincronizador de Tiendas-\>Actualizaciones”: **

![](/media/image327.png)

Para ello, se puede proceder de varias formas:

1.  Creando previamente el fichero de script de base de datos y cargándolo en comerzzia pulsando sobre el botón “Examinar”.

2.  Introduciendo manualmente en el área de trabajo las sentencias SQL.

3.  Cargando en comerzzia el fichero y editándolo desde el área de trabajo.

Tras esta operación, se visualizará la información del fichero por pantalla, disponiendo de las siguientes opciones:

![](/media/image328.png): Permite realizar el envío del fichero a las tiendas seleccionados mediante las opciones explicadas a continuación.

![](/media/image329.png): Elimina la información cargada.

Las actualizaciones dispondrán de las siguientes formas de envío:

  - Seleccionar todas las tiendas activas de la empresa para que la actualización se genere para cada una de ellas y para todas sus cajas. Permite la selección por tipo de sincronización de las tiendas.

  - Seleccionar una tienda y la caja o cajas para las que se crea la actualización.

La configuración de envío se realiza a través de las siguientes opciones:

![](/media/image330.png)

  - **Actualización forzada:** comerzzia aplicará la actualización enviada de forma prioritaria al resto de actualizaciones pendientes para la(s) tienda(s) y caja(s) seleccionadas, anulando las que estén pendientes anteriormente.

  - **Selección de tienda:** Permite seleccionar:
    
      - Todas las tiendas activas
    
      - Todas las tiendas con tipo de sincronización ON-LINE.
    
      - Todas las tiendas con tipo de sincronización OFF-LINE Centralizada.
    
      - Todas las tiendas con tipo de sincronización OFF-LINE Sincronización remota.
    
      - Una tienda concreta, utilizando la ayuda de tiendas para su selección.

  - **Selección de cajas:** Permite seleccionar:
    
      - Todas las cajas activas
    
      - Todas las cajas Máster de la(s) tienda(s) seleccionada(s).
    
      - Todas las cajas Autónomas de la(s) tienda(s) seleccionada(s).
    
      - Selección concreta de cajas Máster/Autónomas. Pudiendo utilizar las opciones disponibles en la barra superior: ![](/media/image331.png).

# ADMINISTRACIÓN DEL GESTOR DE TIENDA

En las tiendas con comerzzia anterior a la versión 3.0 y sincronización remota y manual, estará instalado el Gestor de tienda, que se ejecutará en la propia tienda para la comunicación con la central. Remítase al manual de la versión 2.x de comerzzia para su consulta.

# CONFIGURACIÓN Y ADMINISTRACIÓN DEL INSTORE ENGINE EN TIENDA

En las **tiendas con sincronización OFF-LINE remota**, estará instalado el ISE, que se ejecutará en la propia tienda para la comunicación con la central. Esta aplicación se encarga de consultar y aplicar las actualizaciones que desde la central hayan sido preparadas para ejecutarse sobre dicha tienda, así como de enviar a la central desde la tienda, información generada por ésta, como pueden ser documentos generados o cierres de caja. Esto es, el ISE actúa de intermediario entre la central y la tienda.

Por el contrario, las tiendas OFF-LINE Sincronización Centralizada y ON-LINE no requieren ISE por conectarse directamente con la central mediante los trabajos del sincronizador de tiendas, en el primero de los casos y por no requerir sincronización con la central, en el segundo de los casos.

## Proceso de Instalación

La instalación del InStoreEngine se realiza siempre en paralelo con la instalación del POS Máster/Autónomo de Tienda. El aplicativo será accesible desde el acceso directo de escritorio:

![](/media/image332.png)

## Configuración del InStoreEngine

Este apartado está dirigido al personal de implantación. A continuación se detallará el árbol de directorios y la definición de las propiedades de los ficheros de configuración necesarios para el correcto funcionamiento del InStoreEngine.

### Ruta de trabajo

La ruta de trabajo para la aplicación InStoreEngine se puede definir de diferentes formas. A continuación detallaremos cada una de ellas por orden de importancia. Si en uno de los siguientes pasos se recoge la definición de la ruta de trabajo no se tendrá en cuenta los pasos posteriores para la definición de la ruta de trabajo.

1.  La etiqueta **\<comerzziaHome/\>** en el fichero **comerzzia.xml**.

2.  Definir la variable **COMERZZIA\_HOME** como **variable de la máquina virtual**.

3.  Definir la variable **COMERZZIA\_HOME** como **variable de entorno del sistema**.

Si no se ha definido la ruta de trabajo en alguno de los pasos anteriormente mencionados, la ruta de trabajo se establece por defecto en la ruta del usuario del sistema (**{USER\_HOME}/.comerzzia**).

### Árbol de directorios

Las tres siguientes capturas de pantallas muestran el árbol de directorios para una correcta implantación del InStoreEngine. Se pasará a definir detalladamente las características de cada uno de estos niveles del árbol.

![000151](/media/image333.png)

1 Raíz

En esta captura se muestra el nivel raíz del directorio. En este nivel se encuentra el fichero **InstalacionServicioInStoreEngine.bat** que se encargará de instalar como servicio la aplicación. Por defecto el proceso Java se arranca con 512mb. Si, en algún cliente, por el volumen de datos que maneja, es necesario ampliar memoria, se podrá realizar modificando el parámetro “-Xmx512m” por “-Xmx1024m” dentro del fichero .bat. Para que la modificación de memoria sea efectiva, será necesario parar el servicio, desinstalarlo, volverlo a instalar y reiniciar para que tome los cambios.

En el mismo nivel se encuentra el **jre6** de 32 bits.

El contenido del directorio bin será explicado en la siguiente captura de pantalla.

![000152](/media/image334.png)

2 bin

En este directorio se encuentra:

  - Los ficheros **InStoreEngine.err** e **InStoreEngine.log** son creados por el servicio una vez instalado en el sistema. Mostrará los errores (System.err) y las salidas (System.out) de la aplicación.

  - El fichero **launcher\_config.properties** es un fichero de propiedades. Este fichero es obligatorio. Contiene propiedades necesarias para el lanzador **comerzzia-inStoreEngine-launcher.jar,** además en este fichero podemos definir el puerto de la aplicación. Las propiedades que podemos definir es:
    
      - **svn-url:** Url del repositorio.
    
      - **svn-user:** Usuario del repositorio.
    
      - **svn-password:** Contraseña del repositorio.
    
      - **svn-updateDelayMinutes:** Tiempo en minutos del escaneo por parte del lanzador del directorio versionado. Ejemplo 0.05 minutos son 3 segundos (0.05min\*60=3seg)
    
      - **svn-conflictResolverPolicy:** Cuando se tiene un control de versiones sobre un directorio se pueden provocar una serie de conflictos sobre los ficheros versionados. Con la propiedad **svn-conflictResolverPolicy** definiremos que hacer con estos conflictos cuando se produzcan. Por defecto la aplicación resuelve los conflictos dándole prioridad a nuestros cambios por encima de otros. Los posibles valores para esta propiedad son:
        
          - **MINE\_CONFLICT:** Da prioridad a nuestro trabajo sobre el de otros en aquellos puntos del fichero donde hubiera conflictos.
        
          - **MINE\_FULL:** Da prioridad a nuestro fichero sobre el fichero subido por otros.
        
          - **THEIRS\_CONFLICT:** Da prioridad al trabajo de otros sobre el de nosotros en aquellos puntos del fichero donde hubiera conflictos.
        
          - **THEIRS\_FULL:** Da prioridad al fichero subido por otros sobre nuestro fichero.
    
      - **port:** Puerto de la aplicación.

![000155](/media/image335.png)

  - El lanzador **comerzzia-inStoreEngine-launcher.jar** encargado de desplegar la aplicación en un servidor Jetty. Además comprobará temporalmente (**svn-updateDelay**) si ha habido un cambio de revisión. Si se produjera un cambio se volvería a desplegar la aplicación y actualizar los ficheros en la ruta de trabajo.

  - El fichero **pos\_config.xml** necesario para la ejecución de la aplicación.

  - Los **\*.dll** necesarios para la librería javahl encargada de mantener actualizada el directorio versionado **despliegue**. En la siguiente captura de pantalla veremos más en profundidad este directorio.

![000153](/media/image336.png)

3 despliegue

El directorio de **despliegue** se encontrará versionado. A continuación definiremos cada una de las características y funcionalidades de cada una de sus directorios contenidos y los ficheros necesarios para una correcta ejecución.

  - El directorio **esbConfig** contendrá otra carpeta llamada **contextos** donde se colocarán separadas por carpetas los contextos Mules.

  - El directorio **lib** contendrá todas las librerías externas al war así como aquellos recursos que necesiten estar contenidos en el classpath para la ejecución de la aplicación. En esta carpeta, por ejemplo tendrán que ir las librerías de mule necesarias para ejecutar los contextos.

  - En el directorio **webapps** contendrá los war de la aplicación para que el servidor puede desplegarlos.

  - En la carpeta **webHome** contendrá recursos estáticos.

  - Por último los ficheros **comerzzia.xml** obligatorio para poder ejecutarse y **log4j.xml** necesario para que genere el log de la aplicación. Una vez iniciada la aplicación el log de la aplicación se encontrara en la misma carpeta de despliegue dentro del directorio logs.

## Funcionamiento del InStoreEngine

EL InStoreEngine se arrancará ejecutando el icono de acceso directo del escritorio, o bien el archivo “InStoreEngine.exe” de la carpeta /bin:

La pantalla de acceso al mismo es la siguiente:

![](/media/image337.png)

Tras acceder, con la clave por defecto: “administrador” y usuario “cmz”, se mostrará la pantalla principal, que es la siguiente:

![](/media/image338.png)

La pantalla principal del aplicativo muestra la información de la tienda y caja asociada al POS Máster/Autónomo, y los avisos del sistema que se reciban en la tienda.

Como se puede ver en la pantalla anterior, el menú del InStoreEngine se encuentra dividido en 3 elementos de menú, que permiten la realización de las siguientes posibilidades:

  - **Documentos:** Permite la consulta de todos los documentos emitidos en la Tienda:

![](/media/image339.png)

  - **Sincronización:** A través de este menú se gestionan todos los trabajos de sincronización y procesado de documentos de la tienda con la Central. Este menú a su vez se divide en:
    
    1.  **Sincronización de Tienda:** Desde esta opción de menú es posible consultar los dos tipos de trabajos que se ejecutan desde la tienda, estos son:

<!-- end list -->

  - **Recibir actualizaciones:** Trabajo por el que se reciben las actualizaciones de datos desde la Central y quedan almacenadas en la Tienda. Recibe los archivos de actualización desde la Central. Este trabajo sólo se ejecutará para el caso de una tienda de sincronización remota, puesto que en el caso de una tienda de sincronización manual, estas actualizaciones no se recibirán de forma automática, sino que será necesario copiar y pegar manualmente el archivo de actualización en un directorio específico que será explicado más adelante.
    
      - > **Aplicar actualizaciones:** Trabajo por el que se aplican las actualizaciones recibidas en la base de datos local de la tienda. Este trabajo se ejecutará en ambos tipos de tiendas, puesto que será necesario que la tienda tenga constancia por así decirlo de las actualizaciones generadas por la Central, siendo independiente la forma en que se hayan obtenido estas actualizaciones.

![](/media/image340.png)

2.  **Bus de Integración:** Permite consultar el estado del bus de integración, así como realizar labores de arranque o parada del mismo. Este Bus de integración será necesario cuando en la tienda se disponga de dispositivos adicionales al POS, como el FASTPOS, Pricecheck, Balanzas electrónicas, etiquetas electrónicas, etc…

![](/media/image341.png)

1.  > **Procesamiento de Documentos:** Desde esta opción de menú es posible consultar el estado de proceso de los documentos, según el estado en el que se encuentren. Los documentos que se procesan actualmente son:

<!-- end list -->

  - > **Documentos de venta:** Envía todos los documentos de venta o devolución generados por la tienda a la central para su posterior tratamiento. Este trabajo se ejecutará en los dos tipos de tienda, para que la central tenga conocimiento de ello.

  - > **Cierres de Caja:** Envía todos los cierres de caja a la central para su posterior tratamiento, tal y como se ha explicado anteriormente. Al igual que en el trabajo anterior, la central también deberá tener información sobre los cierres de caja, por lo que también se ejecutará este trabajo para ambas tiendas.

> Se divide en 3 pestañas de consulta:

![](/media/image342.png)

1.  > **Pendientes de procesar:** Documentos pendientes de procesar en la Central.

2.  > **Con Errores:** Documentos que se han intentado procesar pero en los que se ha detectado algún tipo de error.

3.  > **Procesados:** Documentos procesados sin errores.

<!-- end list -->

  - > **Sistema:** A través de este menú, se accede a la gestión del sincronizador y procesador de datos, así como a la configuración asociada al InStoreEngine, que detallamos a continuación:
    
    3.  **Sincronizador:** Permite consultar el estado del sincronizador con la Central, así como realizar labores de arranque o parada del mismo:

![](/media/image343.png)

4.  **Procesador de Datos:** Permite consultar el estado del procesador de Datos, así como realizar labores de arranque o parada del mismo:

![](/media/image344.png)

5.  **Configuración:** Permite consultar y gestionar la configuración del sincronizador de Tiendas y del procesador de Datos, así como gestionar las conexiones a los servicios REST de la Central para la comunicación con las Tiendas:

![](/media/image345.png)
