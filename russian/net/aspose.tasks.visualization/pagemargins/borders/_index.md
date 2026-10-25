---
title: "PageMargins.Borders"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageMargins. Получает или задает позицию, где печатать границы. Может принимать одно из значений перечисления Border."
type: docs
weight: 20
url: /ru/net/aspose.tasks.visualization/pagemargins/borders/
---
## PageMargins.Borders property

Получает или задает позицию, где печатать границы. Может быть одним из значений перечисления [`Border`](../../border/).

```csharp
public Border Borders { get; set; }
```

## Примеры

Показывает, как работать с полями страницы.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// позволяет изменить представление по умолчанию
var margins = project.DefaultView.PageInfo.Margins;

// позволяет изменить поля
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* enum [Border](../../border/)
* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


