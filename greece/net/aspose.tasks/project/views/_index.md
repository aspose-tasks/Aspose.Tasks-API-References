---
title: "Project.Views"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει μια λίστα από αντικείμενα View"
type: docs
weight: 1020
url: /el/net/aspose.tasks/project/views/
---
## Project.Views property

Λαμβάνει μια λίστα από αντικείμενα [`View`](../../view/).

```csharp
public ViewCollection Views { get; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε μια προεπιλεγμένη προβολή έργου.

```csharp
var project = new Project(DataDir + "Project5.mpp");

View view = null;
foreach (var v in project.Views)
{
    if (v.Name == "&Gantt Chart")
    {
        view = v;
    }
}

// ορίστε προεπιλεγμένη προβολή
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Δείτε επίσης

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


