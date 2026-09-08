---
title: "Gridline.Pattern"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Gridline. Получает или задает LinePattern сеточной линии."
type: docs
weight: 40
url: /ru/net/aspose.tasks.visualization/gridline/pattern/
---
## Gridline.Pattern property

Получает или задает [`LinePattern`](../../linepattern/) сеточной линии.

```csharp
public LinePattern Pattern { get; set; }
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

* enum [LinePattern](../../linepattern/)
* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


