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
