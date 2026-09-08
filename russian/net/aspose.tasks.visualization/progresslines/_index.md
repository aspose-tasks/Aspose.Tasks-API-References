---
title: "Класс ProgressLines"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.ProgressLines. Представляет линии прогресса в представлении диаграммы Ганта"
type: docs
weight: 3290
url: /ru/net/aspose.tasks.visualization/progresslines/
---
## ProgressLines class

Представляет линии прогресса в представлении диаграммы Ганта.

```csharp
public class ProgressLines
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [ProgressLines](progresslines/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BeginAtDate](../../aspose.tasks.visualization/progresslines/beginatdate/) { get; set; } | Получает или задает дату, с которой отображаются линии прогресса. |
| [BeginAtProjectStart](../../aspose.tasks.visualization/progresslines/beginatprojectstart/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать линии прогресса с начала даты начала проекта. |
| [DateFormat](../../aspose.tasks.visualization/progresslines/dateformat/) { get; set; } | Получает или задает формат даты ([`DateLabel`](../datelabel/)). |
| [DisplayAtCurrentDate](../../aspose.tasks.visualization/progresslines/displayatcurrentdate/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать линию прогресса на текущую дату. |
| [DisplayAtRecurringIntervals](../../aspose.tasks.visualization/progresslines/displayatrecurringintervals/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать линию прогресса через повторяющиеся интервалы. |
| [DisplaySelected](../../aspose.tasks.visualization/progresslines/displayselected/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать линии прогресса в выбранные даты. |
| [Font](../../aspose.tasks.visualization/progresslines/font/) { get; set; } | Получает или задает шрифт, используемый для подписи линии прогресса. |
| [IsBaselinePlan](../../aspose.tasks.visualization/progresslines/isbaselineplan/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать линии прогресса для базового плана или фактического. |
| [LineColor](../../aspose.tasks.visualization/progresslines/linecolor/) { get; set; } | Получает или задает цвет линии для текущей линии прогресса. |
| [LinePattern](../../aspose.tasks.visualization/progresslines/linepattern/) { get; set; } | Получает или задает шаблон линии текущей линии прогресса. [`LinePattern`](./linepattern/). |
| [OtherLineColor](../../aspose.tasks.visualization/progresslines/otherlinecolor/) { get; set; } | Получает или задает цвет другой линии прогресса. |
| [OtherLinePattern](../../aspose.tasks.visualization/progresslines/otherlinepattern/) { get; set; } | Получает или задает шаблон линии для другой линии прогресса. |
| [OtherProgressPointColor](../../aspose.tasks.visualization/progresslines/otherprogresspointcolor/) { get; set; } | Получает или задает цвет другой точки прогресса. |
| [OtherProgressPointShape](../../aspose.tasks.visualization/progresslines/otherprogresspointshape/) { get; set; } | Получает или задает форму точки прогресса другой линии. |
| [ProgressPointColor](../../aspose.tasks.visualization/progresslines/progresspointcolor/) { get; set; } | Получает или задает цвет точки прогресса. |
| [ProgressPointShape](../../aspose.tasks.visualization/progresslines/progresspointshape/) { get; set; } | Получает или задает форму точки прогресса. [`GanttBarEndShape`](../ganttbarendshape/). |
| [RecurringInterval](../../aspose.tasks.visualization/progresslines/recurringinterval/) { get; set; } | Получает или задает повторяющийся интервал. [`RecurringInterval`](./recurringinterval/). |
| [SelectedDates](../../aspose.tasks.visualization/progresslines/selecteddates/) { get; } | Получает список выбранных дат для отображения линий прогресса. |
| [ShowDate](../../aspose.tasks.visualization/progresslines/showdate/) { get; set; } | Получает или задает значение, указывающее, показывать ли дату для каждой линии прогресса. |

## Примеры

Показывает, как работать с линиями прогресса.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// определим линию прогресса
view.ProgressLines = new ProgressLines();
var progressLines = view.ProgressLines;

// установите дату, с которой отображать линии прогресса. Установим дату статуса проекта.
progressLines.BeginAtDate = project.Get(Prj.StatusDate);
// установите значение, указывающее, отображать ли линии прогресса с начала даты начала проекта
progressLines.BeginAtProjectStart = true;
// установите формат даты (<see cref="T:Aspose.Tasks.Visualization.DateLabel" />).
progressLines.DateFormat = DateLabel.DayDddd;
// установите значение, указывающее, отображать ли линию прогресса на текущую дату.
progressLines.DisplayAtCurrentDate = true;
// установите значение, указывающее, отображать ли линию прогресса через регулярные интервалы.
progressLines.DisplayAtRecurringIntervals = true;
// установите значение, указывающее, отображать ли линии прогресса на выбранных датах
progressLines.DisplaySelected = true;
// установите значение, указывающее, отображать ли линии прогресса для базового плана или фактического.
progressLines.IsBaselinePlan = false;
// установите шрифт, используемый для подписи линии прогресса.
progressLines.Font = new FontDescriptor("Arial", 10);
// установите цвет линии для текущей линии прогресса.
progressLines.LineColor = Color.Aquamarine;
// установите шаблон линии текущей линии прогресса.
progressLines.LinePattern = LinePattern.Dashed;
// установите цвет другой линии прогресса.
progressLines.OtherLineColor = Color.Azure;
// установите шаблон линии для другой линии прогресса.
progressLines.OtherLinePattern = LinePattern.Dotted;
// установите цвет другой точки прогресса.
progressLines.OtherProgressPointColor = Color.Red;
// установите форму точки прогресса другой линии прогресса.
progressLines.OtherProgressPointShape = GanttBarEndShape.Circle;
// установите цвет точки прогресса.
progressLines.ProgressPointColor = Color.Orange;
// установить форму точки прогресса.
progressLines.ProgressPointShape = GanttBarEndShape.Diamond;
// установить повторяющийся интервал.
progressLines.RecurringInterval = new RecurringInterval();
// установить повторяющийся интервал.
progressLines.RecurringInterval.Interval = Interval.Daily;
// установить номер дня
progressLines.RecurringInterval.DailyDayNumber = 1;
// установить значение, указывающее, показывать ли дату для каждой линии прогресса.
progressLines.ShowDate = true;

// давайте проверим линии прогресса
Console.WriteLine("Begin At Date: " + progressLines.BeginAtDate);
Console.WriteLine("Begin At Project Start: " + progressLines.BeginAtProjectStart);
Console.WriteLine("Date Format: " + progressLines.DateFormat);
Console.WriteLine("Display At Current Date: " + progressLines.DisplayAtCurrentDate);
Console.WriteLine("Display At Recurring Intervals: " + progressLines.DisplayAtRecurringIntervals);
Console.WriteLine("Display Selected: " + progressLines.DisplaySelected);
Console.WriteLine("Font: " + progressLines.Font);
Console.WriteLine("Is Baseline Plan: " + progressLines.IsBaselinePlan);
Console.WriteLine("Line Color: " + progressLines.LineColor);
Console.WriteLine("Line Pattern: " + progressLines.LinePattern);
Console.WriteLine("Other Line Color: " + progressLines.OtherLineColor);
Console.WriteLine("Other Line Pattern: " + progressLines.OtherLinePattern);
Console.WriteLine("Other Progress Point Color: " + progressLines.OtherProgressPointColor);
Console.WriteLine("Other Progress Point Shape: " + progressLines.OtherProgressPointShape);
Console.WriteLine("Progress Point Color: " + progressLines.ProgressPointColor);
Console.WriteLine("Progress Point Shape: " + progressLines.ProgressPointShape);
Console.WriteLine("Recurring Interval: " + progressLines.RecurringInterval.Interval);
Console.WriteLine("Recurring Interval DailyDayNumber: " + progressLines.RecurringInterval.DailyDayNumber);
Console.WriteLine("Selected Dates: ");
foreach (var date in progressLines.SelectedDates)
{
    Console.WriteLine("Date: " + date);
}
Console.WriteLine("Show Date: " + progressLines.ShowDate);
Console.WriteLine();

project.Save(OutDir + "WorkWithProgressLines_out.mpp", SaveFileFormat.Mpp);
```

### См. также

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


