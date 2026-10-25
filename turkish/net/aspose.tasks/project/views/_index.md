---
title: "Project.Views"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Project özelliği. View nesnelerinin bir listesini alır"
type: docs
weight: 1020
url: /tr/net/aspose.tasks/project/views/
---
## Project.Views property

[`View`](../../view/) nesnelerinin bir listesini alır.

```csharp
public ViewCollection Views { get; }
```

## Örnekler

Varsayılan proje görünümünü nasıl ayarlayacağınızı gösterir.

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

// varsayılan görünümü ayarla
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Ayrıca Bakınız

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


