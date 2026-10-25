---
title: "ProjectView.GetDefaultResourceUsageView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectView. Включает столбцы ресурсов: Uid, имя, начало, завершение и работа."
type: docs
weight: 50
url: /ru/net/aspose.tasks.visualization/projectview/getdefaultresourceusageview/
---
## ProjectView.GetDefaultResourceUsageView method

Включает столбцы Uid, name, start, finish и work resource.

```csharp
public static ProjectView GetDefaultResourceUsageView()
```

### Возвращаемое значение

представление, которое содержит список [`ResourceViewColumn`](../../resourceviewcolumn/).

## Примеры

Показывает, как сохранить проект с представлением использования ресурсов.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceUsageView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceUsageView_out.pdf", options);
```

### См. также

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


