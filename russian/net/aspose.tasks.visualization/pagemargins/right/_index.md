---
title: "PageMargins.Right"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PageMargins. Получает или задает размер правого поля в сантиметрах"
type: docs
weight: 50
url: /ru/net/aspose.tasks.visualization/pagemargins/right/
---
## PageMargins.Right property

Получает или задает размер правого поля в сантиметрах.

```csharp
public double Right { get; set; }
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

* class [PageMargins](../)
* namespace [Aspose.Tasks.Visualization](../../pagemargins/)
* assembly [Aspose.Tasks](../../../)


