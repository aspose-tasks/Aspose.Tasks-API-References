---
title: "Gridline.Gridline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор Gridline. Инициализирует новый экземпляр класса Gridline."
type: docs
weight: 10
url: /ru/net/aspose.tasks.visualization/gridline/gridline/
---
## Gridline constructor

Инициализирует новый экземпляр класса [`Gridline`](../).

```csharp
public Gridline()
```

## Примеры

Показывает, как работать с линиями сетки при сохранении в визуальных форматах.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // Установите тип линии сетки (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // Установите <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> линии сетки
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### См. также

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


