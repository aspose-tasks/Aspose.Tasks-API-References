---
title: "Prj.ShowProjectSummaryTask"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν θα εμφανιστούν συνοπτικές πληροφορίες για ολόκληρο το έργο σε μια μόνο γραμμή με τη δική του γραμμή σύνοψης εργασίας στην κορυφή της προβολής Gantt Chart"
type: docs
weight: 640
url: /el/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

Καθορίζει εάν θα εμφανιστούν συνοπτικές πληροφορίες για ολόκληρο το έργο σε μία μόνο γραμμή με τη δική της γραμμή σύνοψης εργασίας στην κορυφή της προβολής Γκάντ.

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.ShowProjectSummaryTask.

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


