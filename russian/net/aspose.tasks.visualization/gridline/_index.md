---
title: "Класс Gridline"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Gridline класс. Горизонтальная или вертикальная линия, которая отображается в представлении проекта"
type: docs
weight: 3100
url: /ru/net/aspose.tasks.visualization/gridline/
---
## Gridline class

Горизонтальная или вертикальная линия, отображаемая в представлении проекта.

```csharp
public class Gridline
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Gridline](gridline/)() | Инициализирует новый экземпляр класса `Gridline`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Получает или задает [`Color`](./color/) полосы сетки. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Получает или задает тип полосы сетки ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Получает или задает [`LinePattern`](../linepattern/) полосы сетки. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Возвращает значение хеш-кода для экземпляра класса `Gridline`. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


