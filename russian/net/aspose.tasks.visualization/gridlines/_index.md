---
title: "Класс Gridlines"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.Gridlines. Представляет линии сетки, которые отображаются в представлении GanttChart."
type: docs
weight: 3120
url: /ru/net/aspose.tasks.visualization/gridlines/
---
## Gridlines class

Представляет линии сетки, отображаемые в представлении GanttChart.

```csharp
public class Gridlines
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Gridlines](gridlines/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Interval](../../aspose.tasks.visualization/gridlines/interval/) { get; set; } | Получает или задает число от 0 до 99, определяющее интервал между линиями сетки. |
| [IntervalColor](../../aspose.tasks.visualization/gridlines/intervalcolor/) { get; set; } | Получает или задает цвет вторичных линий сетки. |
| [IntervalPattern](../../aspose.tasks.visualization/gridlines/intervalpattern/) { get; set; } | Получает или задает шаблон линии для вспомогательных линий сетки. |
| [NormalColor](../../aspose.tasks.visualization/gridlines/normalcolor/) { get; set; } | Получает или задает цвет обычных линий сетки. |
| [NormalPattern](../../aspose.tasks.visualization/gridlines/normalpattern/) { get; set; } | Получает или задает шаблон линии для обычных линий сетки. |
| [Type](../../aspose.tasks.visualization/gridlines/type/) { get; set; } | Получает или задает тип линии сетки. |

## Примеры

Показывает, как работать с линиями сетки.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var view = (GanttChartView)project.Views.ToList()[0];

// Позволяет настроить первую линию сетки представления
var gridlines = view.Gridlines[0];
// Устанавливает число от 0 до 99, определяющее интервал между линиями сетки.
gridlines.Interval = 2;
// Устанавливает цвет вспомогательных линий сетки.
gridlines.IntervalColor = Color.Red;
// Устанавливает шаблон линии для вспомогательных линий сетки
gridlines.IntervalPattern = LinePattern.Solid;
// Устанавливает цвет обычных линий сетки
gridlines.NormalColor = Color.Blue;
// Устанавливает шаблон линии для обычных линий сетки
gridlines.NormalPattern = LinePattern.CloseDot;
// Устанавливает тип линии сетки
gridlines.Type = GridlineType.GanttRow;

project.Save(OutDir + "WorkWithGridlines_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


