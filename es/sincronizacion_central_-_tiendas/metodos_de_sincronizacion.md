## Métodos de sincronización {#m-todos-de-sincronizaci-n}

Comerzzia permite sincronizar la información desde central a tiendas y desde tiendas a central utilizando los siguientes métodos:

*   **Conexión Online.** No es necesaria sincronización porque las tiendas acceden directamente a la base de datos de la oficina central por estar siempre online.
*   **Conexión Offline con sincronización Centralizada.** La tienda tiene su propia Base de datos. La actualización se realiza desde el servidor central que accede directamente a la base de datos de la tienda para actualizar o leer sus datos.
*   **Conexión Offline con sincronización Remota.** La tienda tiene su propia Base de datos. La actualización se realiza desde la tienda desde el módulo in-store engine, que es el encargado se solicitar y enviar datos vía webservice a la central.
*   **Conexión Offline con sincronización Remota y POS autónomo**. Igual que el caso anterior, pero se instala una base de datos por cada POS.

### Sincronización Offline Centralizada {#sincronizaci-n-offline-centralizada}

Existe un planificador de tareas en el servidor central para que estas se ejecuten cada cierto tiempo configurable de manera periódica. Existen diferentes tareas para cada tienda. La ejecución de una tarea, abre una conexión con la base de datos de la tienda que corresponda y actualiza sus tablas o lee los registros necesarios para copiarlos en la central.

*   Requisitos: Se requiere visibilidad IP desde la central a cada una de las tiendas. El puerto de la base de datos de cada una de las tiendas debe de estar abierto para que desde la central se pueda conectar a la base de datos de la tienda.
*   Ventajas: El proceso está centralizado y se puede controlar todo desde la central. No requiere instalar módulo de sincronización _in-store engine_ en las tiendas.
*   Inconvenientes: No permite configurar conexión SSL. Se requiere visibilidad IP a cada una de las tiendas y que estas mantengan IP fija. Se requiere que el puerto de las bases de datos de cada tienda esté abierto para acceso desde servidor central.

### Sincronización Offline Remota {#sincronizaci-n-offline-remota}

Descripción: Existe un planificador de tareas en el módulo in-store engine instalado en cada tienda. Estas tareas se ejecutan cada cierto tiempo configurable de manera periódica. La ejecución de una tarea realiza una petición a un webservice de la central vía HTTP enviando datos o solicitando actualizaciones.

*   Requisitos: Se requiere visibilidad IP desde cada tienda a la central para realizar una petición HTTP o HTTPS. Se requiere instalar módulo de sincronización in-store engine en cada tienda.
*   Ventajas: Permite configurar conexión SSL. No requiere IP fijas en las tiendas. Las operaciones se realizan vía webservice sin acceso remoto directo a las bases de datos. La carga de sincronización se encuentra distribuida haciendo más ligero el servidor central.
*   Inconvenientes: Existe un menor control de supervisión por parte del usuario del proceso de sincronización. Al no estar centralizado en un único sitio, se requiere que los módulo in-store engine de cada tienda estén arrancados y funcionando para asegurar que los datos se están actualizando.

### Sincronización Offline Remota con POS Autónomo {#sincronizaci-n-offline-remota-con-pos-aut-nomo}

Descripción: La arquitectura es idéntica al caso anterior, con la salvedad de que se instala una base de datos y un módulo in-store engine en cada terminal POS de la tienda.

*   Requisitos: Se requiere visibilidad IP desde cada POS de la tienda a la central para realizar una petición HTTP o HTTPS. Se requiere instalar módulo de sincronización in-store engine en cada POS de la tienda.
*   Ventajas: Igual que en el caso anterior. Además:
    *   El POS puede funcionar de manera autónoma aunque la red de la tienda deje de funcionar momentáneamente.
    *   Como cada POS tiene su propia base de datos, no requieren conectarse a un POS Máster, pudiendo funcionar todos de manera autónoma.
*   Inconvenientes: Igual que en el caso anterior. Además:
*   Determinadas operaciones no pueden realizarse de manera común en toda la tienda, ya que los datos no son compartidos al existir una base de datos independiente por POS. En general, cualquier operación sobre base de datos desde el POS será invisible para el resto de POS. Por ejemplo:
    *   Si se registra un cliente en un POS sólo se hace en la base de datos de ese POS.
    *   Los POS no pueden consultar los tickets realizados en otro POS.
    *   El cambio de permisos de usuario debe hacerse en cada POS.
    *   El cambio de password de cada usuario debe hacerse en cada POS o desde Backoffice.
*   El proceso de sincronización es más lento y costoso debido a que existen muchas más bases de datos que actualizar.