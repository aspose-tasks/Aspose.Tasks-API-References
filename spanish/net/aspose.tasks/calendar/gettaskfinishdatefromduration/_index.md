---
title: Calendar.GetTaskFinishDateFromDuration
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Calendar método. Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio las partes divididas y la duración.
type: docs
weight: 190
url: /es/net/aspose.tasks/calendar/gettaskfinishdatefromduration/
---
## Calendar.GetTaskFinishDateFromDuration method

Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, las partes divididas y la duración.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| task | Task | La tarea para la que se va a obtener la fecha de finalización. |
| duration | TimeSpan | La duración de la tarea para dividir. |

### Valor_devuelto

Fecha de finalización de la tarea.

### Observaciones

Devuelve DateTime.MinValue si la tarea es resumida, nula o su fecha de inicio no está establecida.

### Ver también

* class [Task](../../task/)
* class [Calendar](../)
* espacio de nombres [Aspose.Tasks](../../calendar/)
* asamblea [Aspose.Tasks](../../../)


