---
title: "Calendar.GetNextWorkingDayStart"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Calcula el inicio del próximo día laborable para la fecha especificada"
type: docs
weight: 180
url: /es/net/aspose.tasks/calendar/getnextworkingdaystart/
---
## Calendar.GetNextWorkingDayStart method

Calcula el inicio del siguiente día laborable para la fecha especificada.

```csharp
public DateTime GetNextWorkingDayStart(DateTime date)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | DateTime | La fecha para la cual obtener el inicio del siguiente día laborable. |

### Valor devuelto

Fecha y hora de inicio del siguiente día laborable.

## Ejemplos

Muestra cómo obtener el inicio del próximo día laborable usando un calendario.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtener el inicio del próximo día laborable (se omite el fin de semana)
var nextWorkingDayStart = calendar.GetNextWorkingDayStart(new DateTime(2020, 4, 10, 13, 0, 0));

// 13 de abril de 2020 9:00 a.m. será impreso
Console.WriteLine(nextWorkingDayStart);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


