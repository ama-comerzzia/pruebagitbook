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
