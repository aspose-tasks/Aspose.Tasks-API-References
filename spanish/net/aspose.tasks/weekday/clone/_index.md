---
title: "WeekDay.Clone"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método WeekDay. Devuelve una copia profunda del día de la semana"
type: docs
weight: 80
url: /es/net/aspose.tasks/weekday/clone/
---
## WeekDay.Clone method

Devuelve una copia profunda del día de la semana.

```csharp
public WeekDay Clone()
```

### Valor devuelto

Devuelve la copia profunda del día de la semana.

## Ejemplos

Muestra cómo clonar un día de la semana.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var calendar = project.Calendars.GetByUid(1);
var weekDay1 = calendar.WeekDays[0];

// crear una copia profunda del día de la semana
var weekDay2 = weekDay1.Clone();

// la igualdad de los calendarios se verifica contra las propiedades del weekday:
// weekday.DayType
// weekday.DayWorking
// weekday.FromDate
// weekday.ToDate
// weekday.WorkingTimes
Console.WriteLine("WeekDay 1 Day Type: " + weekDay1.DayType);
Console.WriteLine("WeekDay 1 Day Working: " + weekDay1.DayWorking);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.FromDate);
Console.WriteLine("WeekDay 1 From Date: " + weekDay1.ToDate);
Console.WriteLine("WeekDay 1 WorkingTimes: " + weekDay1.WorkingTimes);
Console.WriteLine("WeekDay 2 Day Type: " + weekDay2.DayType);
Console.WriteLine("WeekDay 2 Day Working: " + weekDay2.DayWorking);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.FromDate);
Console.WriteLine("WeekDay 2 From Date: " + weekDay2.ToDate);
Console.WriteLine("WeekDay 2 WorkingTimes: " + weekDay2.WorkingTimes);
Console.WriteLine("Are weekdays equal: " + weekDay1.Equals(weekDay2));
Console.WriteLine("Are weekdays equal (by reference): " + ReferenceEquals(weekDay1, weekDay2));
```

### Ver también

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


