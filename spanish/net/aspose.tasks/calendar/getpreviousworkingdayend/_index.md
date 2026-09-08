---
title: "Calendar.GetPreviousWorkingDayEnd"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Calendar. Calcula el final del día laborable anterior a partir de la fecha especificada"
type: docs
weight: 190
url: /es/net/aspose.tasks/calendar/getpreviousworkingdayend/
---
## Calendar.GetPreviousWorkingDayEnd method

Calcula el final del día laborable anterior a partir de la fecha especificada.

```csharp
public DateTime GetPreviousWorkingDayEnd(DateTime date)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fecha | DateTime | la fecha para calcular el final del día laborable anterior. |

### Valor devuelto

El final del día laborable anterior.

## Ejemplos

Muestra cómo obtener el final del día laborable anterior usando un calendario.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// obtener final del día laborable anterior
var previousWorkingDayEnd = calendar.GetPreviousWorkingDayEnd(new DateTime(2020, 4, 10, 13, 0, 0));

// Se imprimirá 9 de abril de 2020 18:00 PM
Console.WriteLine(previousWorkingDayEnd);
```

### Ver también

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


