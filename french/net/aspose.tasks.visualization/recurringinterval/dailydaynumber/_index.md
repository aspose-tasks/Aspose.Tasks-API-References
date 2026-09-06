---
title: "RecurringInterval.DailyDayNumber"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété RecurringInterval. Obtient ou définit le numéro du jour quotidien"
type: docs
weight: 20
url: /fr/net/aspose.tasks.visualization/recurringinterval/dailydaynumber/
---
## RecurringInterval.DailyDayNumber property

Obtient ou définit le numéro du jour quotidien.

```csharp
public int DailyDayNumber { get; set; }
```

## Exemples

Montre comment ajouter un intervalle récurrent quotidien des lignes de progression.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// définir le numéro du jour du modèle quotidien
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// définir une valeur indiquant si un jour est ouvrable pour les lignes de progression quotidiennes.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Voir aussi

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


