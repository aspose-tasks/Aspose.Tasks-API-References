---
title: "Перечисление Border"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Border enum. Указывает тип границ"
type: docs
weight: 2970
url: /ru/net/aspose.tasks.visualization/border/
---
## Border enumeration

Указывает тип границ.

```csharp
public enum Border
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| NoBorder | `0` | Нет границы. |
| AroundEveryPage | `1` | Вокруг каждой страницы. |
| OutsidePages | `2` | На внешних страницах. |

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


