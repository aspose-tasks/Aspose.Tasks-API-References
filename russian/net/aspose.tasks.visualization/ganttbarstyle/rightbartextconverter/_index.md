---
title: "GanttBarStyle.RightBarTextConverter"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство GanttBarStyle. Получает или задает пользовательский конвертер для получения текста, отображаемого справа от полосы задачи. Переопределяет значение свойства RightField."
type: docs
weight: 170
url: /ru/net/aspose.tasks.visualization/ganttbarstyle/rightbartextconverter/
---
## GanttBarStyle.RightBarTextConverter property

Получает или задает пользовательский конвертер для получения текста, отображаемого справа от полосы задачи. Переопределяет значение свойства [`RightField`](../rightfield/).

```csharp
public TaskBarTextConverter RightBarTextConverter { get; set; }
```

## Примечания

Не сохраняется в формате MPP.

## Примеры

Показывает, как использовать пользовательские стили полос в представлении диаграммы Ганта.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Стили полос могут быть специфичными для задачи (расположены в GanttChartView.CustomBarStyles)
// или специфичными для категории (расположены в GanttChartView.BarStyles)
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // В демонстрационных целях мы изменяем стиль задачи с уникальным идентификатором = 4
    // Здесь мы задаём поле (TaskName) для отображения слева от полосы задачи.
    ganttBarStyle.LeftField = Field.TaskName;
    // Здесь мы задаём пользовательский конвертер, чтобы контролировать, какой текст будет отображаться внутри полосы задачи.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // В демонстрационных целях мы изменяем стили, применимые к задачам‑контрольным точкам.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### См. также

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


