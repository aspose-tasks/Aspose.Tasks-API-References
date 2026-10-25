---
title: "Перечисление GanttBarMiddleShape"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.GanttBarMiddleShape enum. Указывает форму середины полосы"
type: docs
weight: 3050
url: /ru/net/aspose.tasks.visualization/ganttbarmiddleshape/
---
## GanttBarMiddleShape enumeration

Указывает среднюю форму полосы.

```csharp
public enum GanttBarMiddleShape
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| LineBottom | `7` | Указывает форму линии, выровненной по нижнему краю. |
| LineMiddle | `6` | Указывает форму линии, выровненной по центру. |
| LineTop | `5` | Указывает форму линии, выровненной по верхнему краю. |
| None | `0` | Указывает пустую форму. |
| RectangleBar | `1` | Указывает форму прямоугольной полосы полной высоты. |
| RectangleBottom | `4` | Указывает форму прямоугольной полосы половинной высоты, выровненной по нижнему краю. |
| RectangleMiddle | `3` | Указывает форму прямоугольной полосы высотой 1/3, выровненной по центру. |
| RectangleTop | `2` | Указывает форму прямоугольной полосы половинной высоты, выровненной по верхнему краю. |

## Примеры

Показывает, как задать пользовательские стили полос в представлении проекта диаграммы Ганта.

```csharp
public void ImplementCustomBarStyle()
{
    try
    {
        var project = new Project(DataDir + "Blank2010.mpp");
        project.RootTask.Children.Add("Task");

        var view = (GanttChartView)project.DefaultView;
        var custom = GetCustomBarStyle();

        // Добавьте пользовательский стиль полосы в коллекцию пользовательских полос представления проекта
        view.CustomBarStyles.Add(custom);

        SimpleSaveOptions options = new MPPSaveOptions
        {
            WriteViewData = true
        };

        project.Save(OutDir + "ImplementCustomBarStyleWriting_out.mpp", options);
    }
    catch (NotSupportedException ex)
    {
        Console.WriteLine(
            ex.Message
            + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http://www.aspose.com/purchase/default.aspx.");
    }
}

public static GanttBarStyle GetCustomBarStyle()
{
    var style = new GanttBarStyle
    {
        ShowForTaskUid = 1,
        MiddleShape = GanttBarMiddleShape.RectangleBottom,
        MiddleFillPattern = GanttBarFillPattern.MediumFill,
        MiddleShapeColor = Color.Blue,

        StartShape = GanttBarEndShape.ArrowDown,
        StartShapeColor = Color.Red,

        EndShape = GanttBarEndShape.ArrowUp,
        EndShapeColor = Color.Yellow,

        LeftField = Field.TaskResourceNames,
        RightField = Field.TaskName,
        TopField = Field.TaskStart,
        BottomField = Field.TaskFinish,
        InsideField = Field.TaskDuration
    };

    return style;
}
```

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


