---
title: "Project.Views"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على قائمة من كائنات View"
type: docs
weight: 1020
url: /ar/net/aspose.tasks/project/views/
---
## Project.Views property

تحصل على قائمة من كائنات [`View`](../../view/).

```csharp
public ViewCollection Views { get; }
```

## الأمثلة

يظهر كيفية تعيين عرض مشروع افتراضي.

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

// تعيين عرض افتراضي
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### انظر أيضًا

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


