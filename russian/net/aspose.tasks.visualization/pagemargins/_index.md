---
title: "Класс PageMargins"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.PageMargins класс. Представляет поля страницы для печати"
type: docs
weight: 3230
url: /ru/net/aspose.tasks.visualization/pagemargins/
---
## PageMargins class

Представляет поля страницы для печати.

```csharp
public class PageMargins
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PageMargins](pagemargins/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Borders](../../aspose.tasks.visualization/pagemargins/borders/) { get; set; } | Получает или задает позицию, где печатать границы. Может быть одним из значений перечисления [`Border`](../border/). |
| [Bottom](../../aspose.tasks.visualization/pagemargins/bottom/) { get; set; } | Получает или задает размер нижнего поля в сантиметрах. |
| [Left](../../aspose.tasks.visualization/pagemargins/left/) { get; set; } | Получает или задает размер левого поля в сантиметрах. |
| [Right](../../aspose.tasks.visualization/pagemargins/right/) { get; set; } | Получает или задает размер правого поля в сантиметрах. |
| [Top](../../aspose.tasks.visualization/pagemargins/top/) { get; set; } | Получает или задает размер верхнего поля в сантиметрах. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


