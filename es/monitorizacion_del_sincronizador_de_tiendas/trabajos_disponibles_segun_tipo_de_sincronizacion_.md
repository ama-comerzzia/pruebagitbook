## Trabajos disponibles según tipo de sincronización de Tienda {#trabajos-disponibles-seg-n-tipo-de-sincronizaci-n-de-tienda}

En función del tipo de sincronización de cada tienda, estarán disponibles el siguiente conjunto de trabajos de sincronización:

1.  **Tienda con sincronización ON-LINE:** No tiene asociada trabajos de sincronización puesto que la tienda comparte la base de datos de la Central.
2.  **Tienda con sincronización OFF-LINE Centralizada:** En este tipo de sincronización, la central conoce la ubicación de la base de datos de la tienda, por lo que, cuando se ejecuten los trabajos indicados a continuación, los datos asociados serán almacenados o consultados directamente en la base de datos de la tienda. En este caso existen 4 trabajos de sincronización, indicados a continuación:
    1.  Enviar Configuración.
    2.  Enviar Artículos.
    3.  Recibir Cierres de Caja.
    4.  Recibir Documentos.
3.  **Tienda con sincronización OFF-LINE Remota:** En este tipo de sincronización, la central desconoce la ubicación de la base de datos de la tienda, por lo que, cuando se ejecuten los trabajos indicados a continuación, los datos asociados serán depositados en un paquete de actualización en la propia central, que será consultado por la tienda cuando se conecte a la misma de forma remota para consultar las actualizaciones asociadas a la misma. En este caso, existen 2 trabajos de sincronización, indicados a continuación:
    1.  Generar Datos Configuración.
    2.  Generar Actualización Artículos.