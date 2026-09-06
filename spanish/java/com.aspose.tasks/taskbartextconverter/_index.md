---
title: "TaskBarTextConverter"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Convertidor personalizado de datos de tareas a texto de barra."
type: docs
weight: 290
url: /es/java/com.aspose.tasks/taskbartextconverter/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.Delegate, com.aspose.ms.System.MulticastDelegate
```
public abstract class TaskBarTextConverter extends System.MulticastDelegate
```

Convertidor personalizado de los datos de la tarea a texto de barra.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [TaskBarTextConverter()](#TaskBarTextConverter--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [invoke(Task task)](#invoke-com.aspose.tasks.Task-) | Convertidor personalizado de los datos de la tarea a texto de barra. |
### TaskBarTextConverter() {#TaskBarTextConverter--}
```
public TaskBarTextConverter()
```


### invoke(Task task) {#invoke-com.aspose.tasks.Task-}
```
public abstract String invoke(Task task)
```


Convertidor personalizado de los datos de la tarea a texto de barra.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tarea para la cual se renderizará el texto de la barra de tareas. |

**Returns:**
java.lang.String - Texto a renderizar para una barra correspondiente a la tarea especificada.
