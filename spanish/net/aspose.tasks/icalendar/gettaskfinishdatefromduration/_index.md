---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ICalendar. Calcula la fecha y hora de finalización de la tarea a partir de sus partes de fecha de inicio y la duración del trabajo."
type: docs
weight: 50
url: /es/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Calcula la fecha y hora de finalización de la tarea a partir de su fecha de inicio, sus partes divididas y la duración del trabajo.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | La tarea para la que se calcula la fecha de finalización. |
| duración | TimeSpan | La duración a calcular. |

### Valor devuelto

Fecha de finalización de la tarea para la fecha de inicio y duración dadas.

## Observaciones

Devuelve DateTime.MinValue si la tarea es resumen, nula o su fecha de inicio no está establecida.

### Ver también

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


