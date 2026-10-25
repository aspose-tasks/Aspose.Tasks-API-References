---
title: "LevelingOptions"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Permite especificar parámetros de nivelación de recursos."
type: docs
weight: 142
url: /es/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Permite especificar parámetros de nivelación de recursos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Inicializa una nueva instancia de la clase [LevelingOptions](../../com.aspose/tasks/levelingoptions). |
## Métodos

| Método | Descripción |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Obtiene un token que puede usarse para cancelar una operación de nivelación de proyecto. |
| [getFinishDate()](#getFinishDate--) | Obtiene la fecha de finalización del período de nivelación. |
| [getLevelingOrder()](#getLevelingOrder--) | Obtiene el orden en que el algoritmo de nivelación retrasa las tareas que tienen sobreasignaciones. |
| [getMessageHandler()](#getMessageHandler--) | Obtiene la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose.Tasks durante la nivelación de recursos. |
| [getMessageLevel()](#getMessageLevel--) | Obtiene el nivel de los mensajes de registro emitidos por Aspose.Tasks durante la nivelación de recursos. |
| [getResources()](#getResources--) | Obtiene la lista de los recursos que serán nivelados. |
| [getStartDate()](#getStartDate--) | Obtiene la fecha de inicio del período de nivelación. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Establece un token que puede usarse para cancelar una operación de nivelación del proyecto. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Establece la fecha de fin del período de nivelación. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | El orden en que el algoritmo de nivelación retrasa tareas que tienen sobreasignaciones. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Establece la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose.Tasks durante la nivelación de recursos. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Establece el nivel de los mensajes de registro emitidos por Aspose.Tasks durante la nivelación de recursos. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Establece la lista de los recursos que serán nivelados. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Establece la fecha de inicio del período de nivelación. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Inicializa una nueva instancia de la clase [LevelingOptions](../../com.aspose/tasks/levelingoptions).

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Obtiene un token que puede usarse para cancelar una operación de nivelación de proyecto.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Obtiene la fecha de fin del período de nivelación. El valor predeterminado es la fecha de finalización del proyecto.

**Returns:**
java.util.Date - fecha de fin del período de nivelación.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Obtiene el orden en que el algoritmo de nivelación retrasa tareas que tienen sobreasignaciones. Después de determinar las tareas que causan la sobreasignación y qué tareas pueden retrasarse, se utiliza el orden especificado para decidir cuál tarea debe retrasarse primero.

**Returns:**
int - el orden en que el algoritmo de nivelación retrasa tareas que tienen sobreasignaciones.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Obtiene la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose.Tasks durante la nivelación de recursos.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Obtiene el nivel de los mensajes de registro emitidos por Aspose.Tasks durante la nivelación de recursos.

**Returns:**
int - nivel de los mensajes de registro emitidos por Aspose.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Obtiene la lista de los recursos que serán nivelados. Si se establece null, todos los recursos del proyecto serán nivelados.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - la lista de los recursos que serán nivelados.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtiene la fecha de inicio del período de nivelación. El valor predeterminado es la fecha de inicio del proyecto.

**Returns:**
java.util.Date - fecha de inicio del período de nivelación.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Establece un token que puede usarse para cancelar una operación de nivelación del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | un token que puede usarse para cancelar una operación de nivelación del proyecto. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Establece la fecha de fin del período de nivelación. El valor predeterminado es la fecha de finalización del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | fecha de fin del período de nivelación. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


El orden en que el algoritmo de nivelación retrasa tareas que tienen sobreasignaciones. Después de determinar las tareas que causan la sobreasignación y qué tareas pueden retrasarse, se utiliza el orden especificado para decidir cuál tarea debe retrasarse primero.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | el orden en que el algoritmo de nivelación retrasa tareas que tienen sobreasignaciones. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Establece la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose.Tasks durante la nivelación de recursos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Establece el nivel de los mensajes de registro emitidos por Aspose.Tasks durante la nivelación de recursos.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | int | nivel de los mensajes de registro emitidos por Aspose. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Establece la lista de los recursos que serán nivelados. Si se establece null, todos los recursos del proyecto serán nivelados.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.List&lt;com.aspose.tasks.Resource&gt; | la lista de los recursos que serán nivelados. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Establece la fecha de inicio del período de nivelación. El valor predeterminado es la fecha de inicio del proyecto.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.util.Date | fecha de inicio del período de nivelación. |

