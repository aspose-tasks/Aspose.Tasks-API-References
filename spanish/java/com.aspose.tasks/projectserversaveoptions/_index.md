---
title: "ProjectServerSaveOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar opciones adicionales cuando el proyecto se guarda en Project Server o Project Online."
type: docs
weight: 227
url: /es/java/com.aspose.tasks/projectserversaveoptions/
---

**Inheritance:**
java.lang.Object
```
public final class ProjectServerSaveOptions
```

Permite especificar opciones adicionales cuando el proyecto se guarda en Project Server o Project Online.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [ProjectServerSaveOptions()](#ProjectServerSaveOptions--) | Inicializa una nueva instancia de la clase [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getPollingInterval()](#getPollingInterval--) | Obtiene el intervalo entre solicitudes de estado de trabajos en cola. |
| [getProjectGuid()](#getProjectGuid--) | Obtiene el identificador único de un proyecto. |
| [getProjectName()](#getProjectName--) | Obtiene el nombre de un proyecto que se muestra en la lista de proyectos de Project Server \\ Project Online. |
| [getTimeout()](#getTimeout--) | Obtiene el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Server. |
| [setPollingInterval(double value)](#setPollingInterval-double-) | Establece el intervalo entre solicitudes de estado de trabajos en cola. |
| [setProjectGuid(UUID value)](#setProjectGuid-java.util.UUID-) | Establece el identificador único de un proyecto. |
| [setProjectName(String value)](#setProjectName-java.lang.String-) | Establece el nombre de un proyecto que se muestra en la lista de proyectos de Project Server \\ Project Online. |
| [setTimeout(double value)](#setTimeout-double-) | Establece el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Server. |
### ProjectServerSaveOptions() {#ProjectServerSaveOptions--}
```
public ProjectServerSaveOptions()
```


Inicializa una nueva instancia de la clase [ProjectServerSaveOptions](../../com.aspose.tasks/projectserversaveoptions).

### getPollingInterval() {#getPollingInterval--}
```
public final double getPollingInterval()
```


Obtiene el intervalo entre solicitudes de estado de trabajos en cola. El valor predeterminado es 2 segundos.

**Returns:**
double - intervalo entre solicitudes de estado de trabajos en cola.
### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Obtiene el identificador único de un proyecto. Debe ser único dentro de la instancia de Project Server \\ Project Online.

**Returns:**
java.util.UUID - identificador único de un proyecto.
### getProjectName() {#getProjectName--}
```
public final String getProjectName()
```


Obtiene el nombre de un proyecto que se muestra en la lista de proyectos de Project Server \\ Project Online. Debe ser único dentro de la instancia de Project Server \\ Project Online. Si el valor se omite, se usará el valor de la propiedad Prj.Name.

**Returns:**
java.lang.String - nombre de un proyecto que se muestra en la lista de proyectos de Project Server \\ Project Online.
### getTimeout() {#getTimeout--}
```
public final double getTimeout()
```


Obtiene el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardado de proyecto por el servicio de procesamiento de colas de Project Server. El valor predeterminado para esta propiedad es 1 minuto.

--------------------

El tiempo de procesamiento puede ser más largo para proyectos grandes o en caso de que la instancia de Project Server esté demasiado ocupada respondiendo a otras solicitudes.

**Returns:**
double - tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardar proyecto por el servicio de procesamiento de cola de Project Server.
### setPollingInterval(double value) {#setPollingInterval-double-}
```
public final void setPollingInterval(double value)
```


Establece el intervalo entre solicitudes de estado de trabajos en cola. El valor predeterminado es 2 segundos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | intervalo entre solicitudes de estado de trabajos en cola. |

### setProjectGuid(UUID value) {#setProjectGuid-java.util.UUID-}
```
public final void setProjectGuid(UUID value)
```


Establece el identificador único de un proyecto. Debe ser único dentro de la instancia de Project Server \ Project Online.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.UUID | identificador único de un proyecto. |

### setProjectName(String value) {#setProjectName-java.lang.String-}
```
public final void setProjectName(String value)
```


Establece el nombre de un proyecto que se muestra en la lista de proyectos de Project Server \ Project Online. Debe ser único dentro de la instancia de Project Server \ Project Online. Si se omite el valor, se utilizará el valor de la propiedad Prj.Name.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | nombre de un proyecto que se muestra en la lista de proyectos de Project Server \ Project Online. |

### setTimeout(double value) {#setTimeout-double-}
```
public final void setTimeout(double value)
```


Establece el tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardar proyecto por el servicio de procesamiento de cola de Project Server. El valor predeterminado para esta propiedad es 1 minuto.

--------------------

El tiempo de procesamiento puede ser más largo para proyectos grandes o en caso de que la instancia de Project Server esté demasiado ocupada respondiendo a otras solicitudes.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | double | tiempo de espera utilizado al esperar el procesamiento de la solicitud de guardar proyecto por el servicio de procesamiento de cola de Project Server. |

