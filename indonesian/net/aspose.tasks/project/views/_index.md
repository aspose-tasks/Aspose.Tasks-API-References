---
title: "Project.Views"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan daftar objek View"
type: docs
weight: 1020
url: /id/net/aspose.tasks/project/views/
---
## Project.Views property

Mendapatkan daftar objek [`View`](../../view/) .

```csharp
public ViewCollection Views { get; }
```

## Contoh

Menampilkan cara mengatur tampilan default proyek.

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

// atur tampilan default
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### Lihat Juga

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


