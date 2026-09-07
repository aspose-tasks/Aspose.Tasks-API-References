---
title: "GanttBarStyle.ShowForCategories"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα GanttBarStyle. Λαμβάνει ή ορίζει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. Ισχύει για γονικά ή κοινά στυλ των μπαρών σε διάγραμμα Gantt, δείτε BarStyles."
type: docs
weight: 200
url: /el/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Λαμβάνει ή ορίζει τις κατηγορίες εργασιών για τις οποίες εφαρμόζεται το στυλ. Ισχύει για γονικά (ή κοινά) στυλ των μπαρών σε διάγραμμα Gantt (δείτε [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


