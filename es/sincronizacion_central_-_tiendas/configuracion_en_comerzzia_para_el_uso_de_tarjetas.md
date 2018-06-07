# CONFIGURACIÓN EN COMERZZIA PARA EL USO DE TARJETAS REGALO {#configuraci-n-en-comerzzia-para-el-uso-de-tarjetas-regalo}

Comerzzia permite realizar la configuración de dos tipos de tarjeta:

*   De importe fijo
*   De importe variable seleccionable en el momento de la compra.

La configuración de ambos tipos de tarjetas regalo se hará siguiendo los siguientes pasos:

1.  **Creación de los artículos asociados a las tarjetas regalo.** En función de la política de tarjetas de cada cliente, se crearán los artículos necesarios para modelar los tipos de tarjeta regalo que maneje. Esto se realizará desde el **“Mantenimiento de artículos”**, creando tantos artículos como tipos de tarjeta regalo de importe fijo tenga y/o un artículo genérico que definirá el tipo de tarjeta de importe variable. A modo de ejemplo, en nuestro caso hemos creado dos artículos, uno para las tarjeta regalo de importe fijo de 30 euros y otro para tarjetas regalo recargables en el momento de la venta:
2.  **Configuración de los códigos de artículos asociados a las tarjetas regalo en cada POS de tienda:** Tras la creación de los artículos, se deberá acceder al fichero **“devices.xml”** de cada POS en el que se soporte la gestión de tarjetas regalo y configurar los códigos de artículos anteriores, tal como se explica de forma detallada en el **“Manual de Instalación en tienda”**. A modo de ejemplo, se muestra captura de pantalla de cómo debe visualizarse los artículos asociados desde el menú de configuración:
3.  **Solicitud de las tarjetas regalo al fabricante:** En paralelo, se solicitarán las tarjetas al fabricante. Comerzzia permite la utilización de tarjetas regalo con código de barras o de banda magnética. No existe ningún tipo de limitación en relación a la codificación asociada a la tarjeta regalo.
4.  **Carga masiva de tarjetas en el sistema:** Tras la recepción de las mismas, estás se deberán cargar en el sistema a través de una operación masiva de carga de las mismas. Este proceso no está disponible actualmente desde el área de administración de Comerzzia, por lo que deberá ser solicitado por el cliente.

**NOTA IMPORTANTE:** La gestión y mantenimiento de las tarjetas regalo así como la consulta de movimientos asociadas a las mismas desde el área de Administración de Comerzzia solo está disponible tras la contratación del módulo Loyalty. En caso contrario, se podrá disponer de esta funcionalidad pero sin posibilidad de gestión por parte de los usuarios.