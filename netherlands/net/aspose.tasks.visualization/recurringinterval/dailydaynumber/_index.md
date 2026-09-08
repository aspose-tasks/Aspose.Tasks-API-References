---
title: "RecurringInterval.DailyDayNumber"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "RecurringInterval-eigenschap. Haalt het dagelijkse dagnummer op of stelt dit in"
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

Haalt of stelt het dagelijkse dagnummer in.

```csharp
public int DailyDayNumber { get; set; }
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


