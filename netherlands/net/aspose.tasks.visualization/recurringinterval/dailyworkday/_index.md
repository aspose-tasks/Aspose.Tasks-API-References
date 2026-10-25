---
title: "RecurringInterval.DailyWorkday"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringInterval-eigenschap. Haalt een waarde op of stelt deze in die aangeeft of een dag een werkdag is voor dagelijkse voortgangslijnen"
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Haalt of stelt een waarde in die aangeeft of een dag een werkdag is voor dagelijkse voortgangslijnen.

```csharp
public bool DailyWorkday { get; set; }
```

## Voorbeelden

Toont hoe je een dagelijks terugkerend interval van voortgangslijnen kunt toevoegen.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// stel het dagelijkse patroon-dagnummer in
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// stel een waarde in die aangeeft of een dag een werkdag is voor dagelijkse voortgangslijnen.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Zie ook

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


