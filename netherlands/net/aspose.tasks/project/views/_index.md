---
title: "Project.Views"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project eigenschap. Haalt een lijst op van View-objecten"
type: docs
weight: 1020
url: /nl/net/aspose.tasks/project/views/
---
## Project.Views property

Haalt een lijst op van [`View`](../../view/) objecten.

```csharp
public ViewCollection Views { get; }
```

## Voorbeelden

Toont hoe een standaard projectweergave in te stellen.

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

// stel standaardweergave in
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Zie ook

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


