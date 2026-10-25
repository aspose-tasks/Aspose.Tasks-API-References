---
title: "Enumeración TaskStatus"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.TaskStatus. Especifica el estado de una tarea"
type: docs
weight: 2460
url: /es/net/aspose.tasks/taskstatus/
---
## TaskStatus enumeration

Especifica el estado de una tarea.

```csharp
public enum TaskStatus
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Undefined | `-1` | Estado de tarea indefinido. |
| Complete | `0` | La tarea está 100 por ciento completa. |
| OnSchedule | `1` | La tarea está dentro del cronograma si el porcentaje acumulado por fases de tiempo está distribuido al menos hasta el día anterior a la fecha de estado. |
| Late | `2` | La tarea está retrasada si el porcentaje acumulado por fases de tiempo no alcanza la medianoche del día anterior a la fecha de estado. |
| Future | `3` | El estado de tarea 'Future' se establece cuando la fecha de inicio de la tarea es mayor que la fecha de estado. |

### Ver también

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


