## Actualización remota de Tiendas {#actualizaci-n-remota-de-tiendas}

Esta opción está disponible desde la V.3.0.3 desde el menú **“Almacén-Tienda”-&gt;Actualización de Tiendas.**

Al igual que se generan actualizaciones de configuración y artículos, desde esta opción de menú se pueden enviar actualizaciones que permitan enviar a las tiendas scripts de base de datos para que sean ejecutados en remoto. Las actualizaciones enviadas estarán disponibles para su consulta desde el menú **“Almacén-Tienda-&gt;Sincronizador de Tiendas-&gt;Actualizaciones”:**

Para ello, se puede proceder de varias formas:

1.  Creando previamente el fichero de script de base de datos y cargándolo en comerzzia pulsando sobre el botón “Examinar”.
2.  Introduciendo manualmente en el área de trabajo las sentencias SQL.
3.  Cargando en comerzzia el fichero y editándolo desde el área de trabajo.

Tras esta operación, se visualizará la información del fichero por pantalla, disponiendo de las siguientes opciones:

: Permite realizar el envío del fichero a las tiendas seleccionados mediante las opciones explicadas a continuación.

: Elimina la información cargada.

Las actualizaciones dispondrán de las siguientes formas de envío:

*   Seleccionar todas las tiendas activas de la empresa para que la actualización se genere para cada una de ellas y para todas sus cajas. Permite la selección por tipo de sincronización de las tiendas.
*   Seleccionar una tienda y la caja o cajas para las que se crea la actualización.

La configuración de envío se realiza a través de las siguientes opciones:

*   **Actualización forzada:** comerzzia aplicará la actualización enviada de forma prioritaria al resto de actualizaciones pendientes para la(s) tienda(s) y caja(s) seleccionadas, anulando las que estén pendientes anteriormente.
*   **Selección de tienda:** Permite seleccionar:
    *   Todas las tiendas activas
    *   Todas las tiendas con tipo de sincronización ON-LINE.
    *   Todas las tiendas con tipo de sincronización OFF-LINE Centralizada.
    *   Todas las tiendas con tipo de sincronización OFF-LINE Sincronización remota.
    *   Una tienda concreta, utilizando la ayuda de tiendas para su selección.
*   **Selección de cajas:** Permite seleccionar:
    *   Todas las cajas activas
    *   Todas las cajas Máster de la(s) tienda(s) seleccionada(s).
    *   Todas las cajas Autónomas de la(s) tienda(s) seleccionada(s).
    *   Selección concreta de cajas Máster/Autónomas. Pudiendo utilizar las opciones disponibles en la barra superior: .