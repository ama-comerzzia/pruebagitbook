## Trabajos de Sincronización Central - Tiendas {#trabajos-de-sincronizaci-n-central-tiendas}

A continuación se detallan los tipos de trabajos de sincronización mencionados anteriormente.

### Trabajo “Enviar Configuración” {#trabajo-enviar-configuraci-n}

Envía o prepara todos los datos de configuración de la tienda, tanto para una tienda que está funcionando, actualizando posibles cambios, como para una tienda “desde cero” que necesita ser “inicializada”.

Este trabajo siempre es forzado. En caso de que se envíe el fichero de configuración a tiendas ya existentes, se actualizará la configuración del POS así como se crearán nuevas variables en el fichero de configuración del POS, si procede.

Los datos de configuración referenciados son:

*   Usuarios (de la tienda) y Perfiles
*   Variables
*   Impuestos
*   Medios de Pago
*   Cajas
*   Información propia de la Tienda.

### Trabajo “Enviar Artículos” {#trabajo-enviar-art-culos}

Envía o prepara todos los datos relacionados con los Artículos:

*   Categorización de los Artículos
*   Artículos
*   Tarifas y Promociones

Los Artículos y Tarifas/Promociones se procesan sujetos a **versiones**, de forma que el sistema gestiona internamente diferencias de información entre Central y Tiendas, a efectos de sincronización de datos.

### Trabajo “Recibir Documentos” {#trabajo-recibir-documentos}

Recepción de los documentos de venta generados en las tiendas. Sólo se reciben, no se procesan en este “trabajo”. Estarán disponibles para su monitorización desde el menú **“Procesamiento de Documentos”.**

### Trabajo “Recibir Cierres de Caja” {#trabajo-recibir-cierres-de-caja}

Recepción de los cierres de las cajas generados en las tiendas. Este trabajo sólo se encarga de recibir los cierres y almacenarlos en el sistema, para su posterior procesado monitorizable desde el menú **“Procesamiento de Documentos”,** ya que los cierres de caja serán tratados por el sistema como un tipo de documento más.

### Trabajo “Generar Actualización de Artículos” {#trabajo-generar-actualizaci-n-de-art-culos}

Genera los datos de actualización de artículos que posteriormente serán sincronizados por el sincronizador remoto.

### Trabajo “Generar Datos Configuración” {#trabajo-generar-datos-configuraci-n}

Genera los datos de configuración que posteriormente serán sincronizados por el sincronizador remoto.