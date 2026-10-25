---
title: "RecurringInterval.DailyWorkday"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad RecurringInterval. Obtiene o establece un valor que indica si un día es laborable para las líneas de progreso diarias"
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Obtiene o establece un valor que indica si un día es laborable para las líneas de progreso diarias.

```csharp
public bool DailyWorkday { get; set; }
```

## Ejemplos

Muestra cómo agregar un intervalo recurrente diario de líneas de progreso.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// establecer el número de día del patrón diario
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// establecer un valor que indique si un día es laborable para las líneas de progreso diarias.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Ver también

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


