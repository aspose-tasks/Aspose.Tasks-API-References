---
title: Project.Views
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets a list of View objects
type: docs
weight: 1020
url: /net/aspose.tasks/project/views/
---
## Project.Views property

Gets a list of [`View`](../../view/) objects.

```csharp
public ViewCollection Views { get; }
```

## Examples

Shows how to set a default project view.

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

// set default view
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### See Also

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


