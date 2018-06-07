## Configuración del InStoreEngine {#configuraci-n-del-instoreengine}

Este apartado está dirigido al personal de implantación. A continuación se detallará el árbol de directorios y la definición de las propiedades de los ficheros de configuración necesarios para el correcto funcionamiento del InStoreEngine.

### Ruta de trabajo {#ruta-de-trabajo}

La ruta de trabajo para la aplicación InStoreEngine se puede definir de diferentes formas. A continuación detallaremos cada una de ellas por orden de importancia. Si en uno de los siguientes pasos se recoge la definición de la ruta de trabajo no se tendrá en cuenta los pasos posteriores para la definición de la ruta de trabajo.

1.  La etiqueta **&lt;comerzziaHome/&gt;** en el fichero **comerzzia.xml**.
2.  Definir la variable **COMERZZIA_HOME** como **variable de la máquina virtual**.
3.  Definir la variable **COMERZZIA_HOME** como **variable de entorno del sistema**.

Si no se ha definido la ruta de trabajo en alguno de los pasos anteriormente mencionados, la ruta de trabajo se establece por defecto en la ruta del usuario del sistema (**{USER_HOME}/.comerzzia**).

### Árbol de directorios {#rbol-de-directorios}

Las tres siguientes capturas de pantallas muestran el árbol de directorios para una correcta implantación del InStoreEngine. Se pasará a definir detalladamente las características de cada uno de estos niveles del árbol.

1 Raíz

En esta captura se muestra el nivel raíz del directorio. En este nivel se encuentra el fichero **InstalacionServicioInStoreEngine.bat** que se encargará de instalar como servicio la aplicación. Por defecto el proceso Java se arranca con 512mb. Si, en algún cliente, por el volumen de datos que maneja, es necesario ampliar memoria, se podrá realizar modificando el parámetro “-Xmx512m” por “-Xmx1024m” dentro del fichero .bat. Para que la modificación de memoria sea efectiva, será necesario parar el servicio, desinstalarlo, volverlo a instalar y reiniciar para que tome los cambios.

En el mismo nivel se encuentra el **jre6** de 32 bits.

El contenido del directorio bin será explicado en la siguiente captura de pantalla.

2 bin

En este directorio se encuentra:

*   Los ficheros **InStoreEngine.err** e **InStoreEngine.log** son creados por el servicio una vez instalado en el sistema. Mostrará los errores (System.err) y las salidas (System.out) de la aplicación.
*   El fichero **launcher_config.properties** es un fichero de propiedades. Este fichero es obligatorio. Contiene propiedades necesarias para el lanzador **comerzzia-inStoreEngine-launcher.jar,** además en este fichero podemos definir el puerto de la aplicación. Las propiedades que podemos definir es:
    *   **svn-url:** Url del repositorio.
    *   **svn-user:** Usuario del repositorio.
    *   **svn-password:** Contraseña del repositorio.
    *   **svn-updateDelayMinutes:** Tiempo en minutos del escaneo por parte del lanzador del directorio versionado. Ejemplo 0.05 minutos son 3 segundos (0.05min*60=3seg)
    *   **svn-conflictResolverPolicy:** Cuando se tiene un control de versiones sobre un directorio se pueden provocar una serie de conflictos sobre los ficheros versionados. Con la propiedad **svn-conflictResolverPolicy** definiremos que hacer con estos conflictos cuando se produzcan. Por defecto la aplicación resuelve los conflictos dándole prioridad a nuestros cambios por encima de otros. Los posibles valores para esta propiedad son:
        *   **MINE_CONFLICT:** Da prioridad a nuestro trabajo sobre el de otros en aquellos puntos del fichero donde hubiera conflictos.
        *   **MINE_FULL:** Da prioridad a nuestro fichero sobre el fichero subido por otros.
        *   **THEIRS_CONFLICT:** Da prioridad al trabajo de otros sobre el de nosotros en aquellos puntos del fichero donde hubiera conflictos.
        *   **THEIRS_FULL:** Da prioridad al fichero subido por otros sobre nuestro fichero.
    *   **port:** Puerto de la aplicación.
*   El lanzador **comerzzia-inStoreEngine-launcher.jar** encargado de desplegar la aplicación en un servidor Jetty. Además comprobará temporalmente (**svn-updateDelay**) si ha habido un cambio de revisión. Si se produjera un cambio se volvería a desplegar la aplicación y actualizar los ficheros en la ruta de trabajo.
*   El fichero **pos_config.xml** necesario para la ejecución de la aplicación.
*   Los ***.dll** necesarios para la librería javahl encargada de mantener actualizada el directorio versionado **despliegue**. En la siguiente captura de pantalla veremos más en profundidad este directorio.

3 despliegue

El directorio de **despliegue** se encontrará versionado. A continuación definiremos cada una de las características y funcionalidades de cada una de sus directorios contenidos y los ficheros necesarios para una correcta ejecución.

*   El directorio **esbConfig** contendrá otra carpeta llamada **contextos** donde se colocarán separadas por carpetas los contextos Mules.
*   El directorio **lib** contendrá todas las librerías externas al war así como aquellos recursos que necesiten estar contenidos en el classpath para la ejecución de la aplicación. En esta carpeta, por ejemplo tendrán que ir las librerías de mule necesarias para ejecutar los contextos.
*   En el directorio **webapps** contendrá los war de la aplicación para que el servidor puede desplegarlos.
*   En la carpeta **webHome** contendrá recursos estáticos.
*   Por último los ficheros **comerzzia.xml** obligatorio para poder ejecutarse y **log4j.xml** necesario para que genere el log de la aplicación. Una vez iniciada la aplicación el log de la aplicación se encontrara en la misma carpeta de despliegue dentro de la directorio logs.