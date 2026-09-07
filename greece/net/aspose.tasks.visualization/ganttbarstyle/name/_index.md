---
title: "GanttBarStyle.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GanttBarStyle ιδιότητα. Λαμβάνει ή ορίζει ένα όνομα του στυλ"
type: docs
weight: 150
url: /el/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Λαμβάνει ή ορίζει το όνομα του στυλ.

```csharp
public string Name { get; set; }
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


