---
title: "RecurringInterval.DailyWorkday"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα RecurringInterval. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν μια ημέρα είναι εργάσιμη για τις καθημερινές γραμμές προόδου"
type: docs
weight: 30
url: /el/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν μια ημέρα είναι εργάσιμη για τις ημερήσιες γραμμές προόδου.

```csharp
public bool DailyWorkday { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε καθημερινό επαναλαμβανόμενο διάστημα γραμμών προόδου.

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// ορίστε τον αριθμό ημέρας του καθημερινού προτύπου
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// ορίστε μια τιμή που υποδεικνύει εάν μια ημέρα είναι εργάσιμη για τις καθημερινές γραμμές προόδου.
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### Δείτε επίσης

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


