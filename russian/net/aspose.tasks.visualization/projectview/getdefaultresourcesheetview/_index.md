---
title: "ProjectView.GetDefaultResourceSheetView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод ProjectView. Включает столбцы ресурса Uid, resource, name, type, material, label, initials, group, max units, standard rate, overtime rate, cost per use, accrue at, base calendar и code"
type: docs
weight: 40
url: /ru/net/aspose.tasks.visualization/projectview/getdefaultresourcesheetview/
---
## ProjectView.GetDefaultResourceSheetView method

Включает столбцы UID, имя ресурса, тип, метку материала, инициалы, группу, максимальное количество, стандартную ставку, ставку за сверхурочную работу, стоимость за использование, начисление, базовый календарь и код ресурса.

```csharp
public static ProjectView GetDefaultResourceSheetView()
```

### Возвращаемое значение

представление, которое содержит список [`ResourceViewColumn`](../../resourceviewcolumn/).

## Примеры

Показывает, как сохранить проект с представлением листа ресурсов.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.Months,
    View = ProjectView.GetDefaultResourceSheetView()
};

project.Save(OutDir + "WorkWithProjectView_ResourceSheetView_out.pdf", options);
```

### См. также

* class [ProjectView](../)
* namespace [Aspose.Tasks.Visualization](../../projectview/)
* assembly [Aspose.Tasks](../../../)


