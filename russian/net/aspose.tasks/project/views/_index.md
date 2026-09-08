---
title: "Project.Views"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Возвращает список объектов View."
type: docs
weight: 1020
url: /ru/net/aspose.tasks/project/views/
---
## Project.Views property

Возвращает список объектов [`View`](../../view/).

```csharp
public ViewCollection Views { get; }
```

## Примеры

Показывает, как установить представление проекта по умолчанию.

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

// установить представление по умолчанию
project.DefaultView = view;

project.Save(OutDir + @"SaveGantChartView_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### См. также

* class [ViewCollection](../../viewcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


