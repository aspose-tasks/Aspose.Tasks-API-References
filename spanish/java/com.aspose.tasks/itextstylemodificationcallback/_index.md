---
title: "ITextStyleModificationCallback"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una devolución de llamada que se invoca antes de que TextStyle se aplique a una celda de tabla."
type: docs
weight: 383
url: /es/java/com.aspose.tasks/itextstylemodificationcallback/
---
```
public interface ITextStyleModificationCallback
```

Representa una devolución de llamada que se invoca antes de que TextStyle se aplique a una celda de tabla.
## Métodos

| Método | Descripción |
| --- | --- |
| [beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)](#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-) | El método que se llamará antes de renderizar una celda de tabla para una fila de tarea en las siguientes vistas: 'Gantt Chart', 'Task Sheet', 'Task Usage'. |
### beforeTaskTextStyleApplied(TaskTextStyleEventArgs args) {#beforeTaskTextStyleApplied-com.aspose.tasks.TaskTextStyleEventArgs-}
```
public abstract void beforeTaskTextStyleApplied(TaskTextStyleEventArgs args)
```


El método que se llamará antes de renderizar una celda de tabla para una fila de tarea en las siguientes vistas: 'Gantt Chart', 'Task Sheet', 'Task Usage'.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| args | [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs) | El objeto [TaskTextStyleEventArgs](../../com.aspose.tasks/tasktextstyleeventargs). |

