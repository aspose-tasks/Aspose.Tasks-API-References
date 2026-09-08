---
title: "Перечисление GanttBarEndShape"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Visualization.GanttBarEndShape. Представляет форму конца в полосах и точках прогресса в линиях прогресса"
type: docs
weight: 3030
url: /ru/net/aspose.tasks.visualization/ganttbarendshape/
---
## GanttBarEndShape enumeration

Представляет конечную форму в полосах и точках прогресса в линиях прогресса.

```csharp
public enum GanttBarEndShape
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| ArrowDown | `14` | Указывает форму конца полосы Gantt в виде стрелки, указывающей вниз. |
| ArrowUp | `8` | Указывает форму конца полосы Gantt в виде стрелки, указывающей вверх. |
| CaretDownTop | `9` | Указывает форму конца полосы Gantt в виде каретки, указывающей вниз, на верхней половине полосы. |
| CaretUpBottom | `10` | Указывает форму конца полосы Gantt в виде каретки, указывающей вверх, на нижней половине полосы. |
| Circle | `19` | Указывает форму конца полосы Gantt в виде круга. |
| CircleArrowDown | `18` | Указывает форму конца полосы Gantt в виде окружённой стрелки, указывающей вниз. |
| CircleArrowUp | `17` | Указывает форму конца полосы Gantt в виде окружённой стрелки, указывающей вверх. |
| CircleDiamond | `13` | Указывает форму конца полосы Gantt в виде окружённого ромба. |
| CircleTriangleDown | `16` | Указывает форму конца полосы Gantt в виде окружённого треугольника, указывающего вниз. |
| CircleTriangleUp | `15` | Указывает форму конца полосы Gantt в виде окружённого треугольника, указывающего вверх. |
| Diamond | `3` | Указывает форму конца полосы Gantt в виде ромба. |
| HouseDown | `2` | Указывает форму конца полосы Gantt в виде перевёрнутого дома. |
| HouseUp | `1` | Указывает форму конца полосы Gantt в виде дома. |
| LeftBracket | `21` | Указывает форму конца полосы Gantt в виде левой скобки. |
| LeftFade | `23` | Указывает форму конца полосы Gantt в виде левого затухания. |
| LineShape | `11` | Указывает форму конца полосы Gantt в виде линии. |
| NoBarEndShape | `0` | Указывает отсутствие формы конца полосы Gantt. |
| RightBracket | `22` | Указывает форму конца полосы Gantt в виде правой скобки. |
| RightFade | `24` | Указывает форму конца полосы Gantt в виде правого затухания. |
| Square | `12` | Указывает форму конца полосы Gantt в виде квадрата. |
| Star | `20` | Указывает форму конца полосы Gantt в виде звезды. |
| TriangleDown | `5` | Указывает форму конца полосы Gantt в виде треугольника, указывающего вниз. |
| TriangleLeft | `7` | Указывает форму конца полосы Ганта в виде треугольника, указывающего влево. |
| TriangleRight | `6` | Указывает форму конца полосы Ганта в виде треугольника, указывающего вправо. |
| TriangleUp | `4` | Указывает форму конца полосы Gantt в виде окружённого треугольника, указывающего вверх. |

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


