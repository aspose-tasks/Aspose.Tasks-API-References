---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttBarStyle ιδιότητα. Λαμβάνει ή ορίζει μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. Εφαρμόζεται για στυλ συγκεκριμένων εργασιών των γραμμών σε διάγραμμα Gantt, δείτε CustomBarStyles"
type: docs
weight: 210
url: /el/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Λαμβάνει ή ορίζει μοναδικό Id μιας εργασίας για την οποία εφαρμόζεται το στυλ. Εφαρμόζεται για στυλ συγκεκριμένων εργασιών των γραμμών σε διάγραμμα Gantt (δείτε [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις κατηγορίες ShowFor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// εργαστείτε με το έργο...
```

### Δείτε επίσης

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


