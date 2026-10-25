---
title: "Prj.MinutesPerWeek"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El número de minutos por semana"
type: docs
weight: 480
url: /es/net/aspose.tasks/prj/minutesperweek/
---
## Prj.MinutesPerWeek field

El número de minutos por semana.

```csharp
public static readonly Key<int, PrjKey> MinutesPerWeek;
```

## Ejemplos

Muestra cómo leer/escribir las propiedades de los días de la semana del proyecto.

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// Establecer propiedades de los días de la semana
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// Mostrar propiedades de los días de la semana
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


