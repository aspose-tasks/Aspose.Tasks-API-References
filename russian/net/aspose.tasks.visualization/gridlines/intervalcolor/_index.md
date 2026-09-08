---
title: "Gridlines.IntervalColor"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Gridlines. Возвращает или задает цвет вторичных линий сетки"
type: docs
weight: 30
url: /ru/net/aspose.tasks.visualization/gridlines/intervalcolor/
---
## Gridlines.IntervalColor property

Получает или задает цвет вторичных линий сетки.

```csharp
public Color IntervalColor { get; set; }
```

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

* class [Gridlines](../)
* namespace [Aspose.Tasks.Visualization](../../gridlines/)
* assembly [Aspose.Tasks](../../../)


