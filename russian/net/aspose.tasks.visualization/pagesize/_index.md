---
title: "Перечисление PageSize"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.PageSize enum. Указывает размер страницы"
type: docs
weight: 3250
url: /ru/net/aspose.tasks.visualization/pagesize/
---
## PageSize enumeration

Указывает размер страницы.

```csharp
public enum PageSize
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Letter | `0` | Размер страницы Letter в пунктах: 792 × 612 |
| Ledger | `1` | Размер страницы Ledger в пунктах: 1224 × 792 |
| A0 | `2` | Размер страницы A0 в пунктах: 3371 × 2384 |
| A1 | `3` | Размер страницы A1 в пунктах: 2384 × 1685 |
| A2 | `4` | Размер страницы A2 в пунктах: 1684 × 1190 |
| A3 | `5` | Размер страницы A3 в пунктах: 1190 × 842 |
| A4 | `6` | Размер страницы A4 в пунктах: 842 × 595 |
| DefinedInView | `7` | Используйте размер страницы, определенный в [`PageSettings`](../pagesettings/) представления (View.PageInfo.PageSettings). |

## Примеры

Показывает, как установить значение, указывающее, что подзадачи на полосе сводной задачи должны быть свернуты.

```csharp
var project = new Project(DataDir + "Project2.mpp");

project.DisplayOptions.ShowProjectSummaryTask = true;
project.Set(Prj.ShowProjectSummaryTask, true);

var options = new PdfSaveOptions
{
    PresentationFormat = PresentationFormat.GanttChart,
    FitContent = true,
    RollUpGanttBars = true,

    // ИЛИ
    // options.RollUpGanttBars = false;
    // DrawNonWorkingTime = true,
    PageSize = PageSize.A3
};

project.Save(OutDir + "RenderGanttChartWithBarsRolledUp_out.pdf", options);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


