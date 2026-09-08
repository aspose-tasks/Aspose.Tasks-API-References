---
title: "Перечисление GridlineType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.GridlineType. Тип линии сетки"
type: docs
weight: 3110
url: /ru/net/aspose.tasks.visualization/gridlinetype/
---
## GridlineType enumeration

Тип линии сетки.

```csharp
public enum GridlineType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| GanttRow | `0` | Указывает линию сетки типа строка диаграммы Ганта. |
| TopTierColumn | `1` | Указывает линию сетки типа столбец верхнего уровня. |
| BottomTierColumn | `2` | Указывает линию сетки типа столбец нижнего уровня. |
| SheetRow | `3` | Указывает линию сетки типа строка листа. |
| SheetColumn | `4` | Указывает линию сетки типа столбец листа. |
| UsageRow | `5` | Указывает линию сетки типа строка использования. |
| UsageColumn | `6` | Указывает линию сетки типа столбец использования. |
| GanttTitleVertical | `7` | Указывает вертикальный тип линии сетки заголовка диаграммы Ганта. |
| GanttTitleHorizontal | `8` | Указывает горизонтальный тип линии сетки заголовка диаграммы Ганта. |
| BarRows | `9` | Указывает тип линии сетки строк полос. |
| GanttProjectStart | `10` | Указывает тип линии сетки начала проекта Ганта. |
| GanttProjectFinish | `11` | Указывает тип линии сетки завершения проекта Ганта. |
| GanttStatusDate | `12` | Указывает тип линии сетки статуса даты Gantt. |
| GanttCurrentDate | `13` | Указывает тип линии сетки текущей даты Gantt. |
| GanttPageBreaks | `14` | Указывает тип линии сетки разрывов страниц Gantt. |
| MiddleTierColumn | `15` | Указывает тип линии сетки столбца среднего уровня. |

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


