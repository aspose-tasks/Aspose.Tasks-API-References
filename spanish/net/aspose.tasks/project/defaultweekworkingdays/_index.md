---
title: "Project.DefaultWeekWorkingDays"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene la instancia de la clase WeekDayCollection que representa una colección de los días laborables semanales predeterminados del proyecto y sus horarios de trabajo."
type: docs
weight: 370
url: /es/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

Obtiene la instancia de la clase [`WeekDayCollection`](../../weekdaycollection/) que representa una colección de los días laborables semanales predeterminados del proyecto y sus horarios de trabajo.

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### Valor devuelto

La instancia de la clase [`WeekDayCollection`](../../weekdaycollection/) que contiene una lista de objetos [`WeekDay`](../../weekday/).

## Observaciones

Los datos solo se encuentran en archivos mpp (no en xml).

## Ejemplos

Muestra cómo obtener el día laborable semanal predeterminado.

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### Ver también

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


