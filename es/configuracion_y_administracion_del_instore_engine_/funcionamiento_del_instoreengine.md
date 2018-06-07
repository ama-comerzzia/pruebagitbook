## Funcionamiento del InStoreEngine {#funcionamiento-del-instoreengine}

EL InStoreEngine se arrancará ejecutando el icono de acceso directo del escritorio, o bien el archivo “InStoreEngine.exe” de la carpeta /bin:

La pantalla de acceso al mismo es la siguiente:

Tras acceder, con la clave por defecto: “administrador” y usuario “cmz”, se mostrará la pantalla principal, que es la siguiente:

La pantalla principal del aplicativo muestra la información de la tienda y caja asociada al POS Máster/Autónomo, y los avisos del sistema que se reciban en la tienda.

Como se puede ver en la pantalla anterior, el menú del InStoreEngine se encuentra dividido en 3 elementos de menú, que permiten la realización de las siguientes posibilidades:

*   **Documentos:** Permite la consulta de todos los documentos emitidos en la Tienda:
*   **Sincronización:** A través de este menú se gestionan todos los trabajos de sincronización y procesado de documentos de la tienda con la Central. Este menú a su vez se divide en:
    1.  **Sincronización de Tienda:** Desde esta opción de menú es posible consultar los dos tipos de trabajos que se ejecutan desde la tienda, estos son:
*   **Recibir actualizaciones:** Trabajo por el que se reciben las actualizaciones de datos desde la Central y quedan almacenadas en la Tienda. Recibe los archivos de actualización desde la Central. Este trabajo sólo se ejecutará para el caso de una tienda de sincronización remota, puesto que en el caso de una tienda de sincronización manual, estas actualizaciones no se recibirán de forma automática, sino que será necesario copiar y pegar manualmente el archivo de actualización en un directorio específico que será explicado más adelante.
    *   *   **Aplicar actualizaciones:** Trabajo por el que se aplican las actualizaciones recibidas en la base de datos local de la tienda. Este trabajo se ejecutará en ambos tipos de tiendas, puesto que será necesario que la tienda tenga constancia por así decirlo de las actualizaciones generadas por la Central, siendo independiente la forma en que se hayan obtenido estas actualizaciones.
    1.  **Bus de Integración:** Permite consultar el estado del bus de integración, así como realizar labores de arranque o parada del mismo. Este Bus de integración será necesario cuando en la tienda se disponga de dispositivos adicionales al POS, como el FASTPOS, Pricecheck, Balanzas electrónicas, etiquetas electrónicas, etc…
    2.  **Procesamiento de Documentos:** Desde esta opción de menú es posible consultar el estado de proceso de los documentos, según el estado en el que se encuentren. Los documentos que se procesan actualmente son:
*   **Documentos de venta:** Envía todos los documentos de venta o de devolución generados por la tienda a la central para su posterior tratamiento. Este trabajo se ejecutará en los dos tipos de tienda, para que la central tenga conocimiento de ello.
*   **Cierres de Caja:** Envía todos los cierres de caja a la central para su posterior tratamiento, tal y como se ha explicado anteriormente. Al igual que en el trabajo anterior, la central también deberá tener información sobre los cierres de caja, por lo que también se ejecutará este trabajo para ambas tiendas. Se divide en 3 pestañas de consulta:
    1.  **Pendientes de procesar:** Documentos pendientes de procesar en la Central.
    2.  **Con Errores:** Documentos que se han intentado procesar pero en los que se ha detectado algún tipo de error.
    3.  **Procesados:** Documentos procesados sin errores.
*   **Sistema:** A través de este menú, se accede a la gestión del sincronizador y procesador de datos, así como a la configuración asociada al InStoreEngine, que detallamos a continuación:
    1.  **Sincronizador:** Permite consultar el estado del sincronizador con la Central, así como realizar labores de arranque o parada del mismo:
    2.  **Procesador de Datos:** Permite consultar el estado del procesador de Datos, así como realizar labores de arranque o parada del mismo:
    3.  **Configuración:** Permite consultar y gestionar la configuración del sincronizador de Tiendas y del procesador de Datos, así como gestionar las conexiones a los servicios REST de la Central para la comunicación con las Tiendas: