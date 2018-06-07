## Detalle de cada Interfaz disponible en el Sincronizador de Tiendas {#detalle-de-cada-interfaz-disponible-en-el-sincronizador-de-tiendas}

En las interfaces descritas a continuación, se visualiza el listado de trabajos de sincronización organizado por diferentes criterios. Para cada trabajo, se podrá visualizar la siguiente información (campos) en pantalla:

*   Trabajo: nombre del Trabajo listado.
*   Tienda: código de la tienda asociada al Trabajo de sincronización.
*   Descripción: Nombre descriptivo asociado a la tienda.
*   Estado:

Arrancado

Parado

Pausado

*   Fecha de Inicio: Cuándo se arrancó el trabajo.
*   Fecha de Próxima Ejecución: según programación (“ejecutar periódicamente”) o indicada manualmente en la edición del Trabajo.
*   Intervalo: según programación (“ejecutar periódicamente”).
*   Fecha de Última Ejecución: Cuándo se ejecutó por última vez.
*   Resultado:

Trabajo realizado correctamente.

El Trabajo no se ha podido realizar / Trabajo con errores.

A continuación se detallan las diferentes vistas disponibles desde el Menú.

### Listado de Trabajos de Sincronización: Vista Trabajos por Tipo {#listado-de-trabajos-de-sincronizaci-n-vista-trabajos-por-tipo}

El monitor nos ofrece la relación de trabajos de sincronización, agrupados, en esta vista, por tipologías de trabajos:

*   Tipo Trabajo “Enviar Artículos”:
*   Tipo Trabajo “Enviar Configuración”:
*   Tipo Trabajo “Generar Actualización de Artículos”
*   Tipo Trabajo “Generar Datos de Configuración”
*   Tipo Trabajo “Recibir Cierres de Cajas”
*   Tipo Trabajo “Recibir Documentos”

### Listado de Trabajos de Sincronización: Vista Trabajos por Tiendas {#listado-de-trabajos-de-sincronizaci-n-vista-trabajos-por-tiendas}

El monitor nos ofrece la relación de trabajos de sincronización, agrupados, en esta vista, por Tiendas:

### Listado de Trabajos de Sincronización: Vista Actualizaciones {#listado-de-trabajos-de-sincronizaci-n-vista-actualizaciones}

Existe la posibilidad de consultar todas las actualizaciones generadas para todas las tiendas, conociendo el estado de dicha actualización, así como poder descargar el fichero xml que corresponde a la actualización. Se pueden filtrar los resultados obtenidos indicando la tienda y las fechas para las que queremos obtener las actualizaciones en el panel de búsqueda.

El listado ofrece la siguiente información para cada actualización generada:

*   Tienda: Código de almacén asociado a la tienda
*   Descripción: Descripción de la tienda
*   ID: Identificador único asociado al paquete de actualización.
*   Tipo: Tipo de actualización (artículos o configuración)
*   Fecha Generación: Fecha en la que se generó la actualización
*   Fecha Transmisión: Fecha en la que la actualización ha sido transmitida. Si no muestra información, es que la actualización está pendiente de ser transmitida.
*   Fecha Aplicación: Fecha en la que la actualización ha sido aplicada en la tienda. Si no existe, es que la actualización todavía no ha sido aplicada.
*   Estado: Resultado de la aplicación de la actualización. Sus posibles valores son:

Pendiente

Aplicada

Errónea

*   Forzada: Muestra información sobre si la actualización ha sido forzada de forma manual a través del botón de ejecución inmediata o no.
*   Acciones: Ofrece al usuario un conjunto de acciones disponibles sobre la actualización:
    *   : la posibilidad de obtener el fichero correspondiente a la actualización en formato xml. Para descargar el fichero, pulsar sobre el icono .
    *   : eliminar la actualización seleccionada.
    *   : Anula la actualización seleccionada.

### Listado de Trabajos de Sincronización: Consulta de Trabajos {#listado-de-trabajos-de-sincronizaci-n-consulta-de-trabajos}

En esta pestaña se puede ver un formulario de consulta en la línea del resto de pantallas de consulta de la aplicación.

Se mostrarán todos los trabajos existentes en función de los filtros introducidos en el bloque de búsqueda, pudiéndose actualizar los resultados de dicha búsqueda. Los filtros mencionados son los siguientes:

*   Tienda (desde - hasta), obtenidas mediante la ayuda correspondiente.
*   Agrupado, muestra los valores definidos para este campo mediante un desplegable.
*   Tipo de Trabajo.
*   Estado.
*   Trabajo con Errores, filtro que hará que se muestren o no aquellos trabajos que han presentado o no, errores en su ejecución, respectivamente.

Para poder visualizar los resultados en modo ficha, bastará con hacer click sobre el botón . Si además se pretende planificar la ejecución de dicho trabajo se pulsará sobre el botón .

La pantalla de detalle de un trabajo es la siguiente:

En caso de editar dicha pantalla, se mostrará la fecha y la hora de la próxima ejecución del trabajo en cuestión.