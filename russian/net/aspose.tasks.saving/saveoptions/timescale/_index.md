---
title: "SaveOptions.Timescale"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство SaveOptions. Получает или задает значение Timescale, которое используется для управления тем, как шкала времени (если присутствует) рендерится при сохранении проекта в графическом формате."
type: docs
weight: 200
url: /ru/net/aspose.tasks.saving/saveoptions/timescale/
---
## SaveOptions.Timescale property

Получает или задает значение `Timescale`, которое используется для управления тем, как шкала времени (если присутствует) рендерится при сохранении проекта в графическом формате.

```csharp
public Timescale Timescale { get; set; }
```

## Примеры

Показывает, как установить минимальный период времени для рендеринга. Значение по умолчанию — <see cref=\"P:Aspose.Tasks.Saving.SaveOptions.Timescale\">Days</see>.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// Сохранить в виде изображения одной страницы (Timescale.days по умолчанию)
project.Save(OutDir + "NewProductDevDays_out.jpeg", new ImageSaveOptions(SaveFileFormat.Jpeg));

// Сохранить в виде изображения одной страницы (Timescale.ThirdsOfMonths)
var options = new ImageSaveOptions(SaveFileFormat.Jpeg)
{
    Timescale = Timescale.ThirdsOfMonths
};

project.Save(OutDir + "NewProductDevThirdsOfMonths_out.jpeg", options);

// Сохранить в виде изображения одной страницы (Timescale.Months)
options.Timescale = Timescale.Months;
project.Save(OutDir + "NewProductDevMonths_out.jpeg", options);
```

Показывает, как работать с уровнями шкалы времени через параметры сохранения.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

GanttChartView ganttChartView = (GanttChartView) project.Views.ToList()[0];

// установить уровни шкалы времени представления диаграммы Ганта
ganttChartView.MiddleTimescaleTier.Unit = TimescaleUnit.Months;
ganttChartView.MiddleTimescaleTier.Count = 1;
ganttChartView.MiddleTimescaleTier.Label = DateLabel.MonthMmmm;

ganttChartView.BottomTimescaleTier.Unit = TimescaleUnit.Days;
ganttChartView.BottomTimescaleTier.Count = 1;
ganttChartView.BottomTimescaleTier.Label = DateLabel.DayDddDd;

// ...
var options = new ImageSaveOptions(SaveFileFormat.Png)
{
    Timescale = Timescale.DefinedInView
};

// ...

// сохранить проект как изображение
project.Save(OutDir + "WorkWithTimescaleTier_out.png", options);
```

Показывает, как отобразить представление использования задач с настройками шкалы времени, определенными в настройках представления.

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = project.Views.ToList()[2] as TaskUsageView;

view.TopTimescaleTier.Unit = TimescaleUnit.None;

view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddMDd;
view.MiddleTimescaleTier.Count = 1;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayMmDd;
view.BottomTimescaleTier.Count = 1;

// Определите SaveOptions и укажите, что следует использовать настройки масштаба времени TaskUsageView.
SaveOptions options = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    PresentationFormat = PresentationFormat.TaskUsage
};

project.Save(OutDir + "TaskUsageView_CustomTimescale_out.pdf", options);
```

Показывает, как изменить уровни шкалы времени.

```csharp
var project = new Project();

// Инициализировать представление диаграммы Ганта
var view = new GanttChartView
{
    TopTimescaleTier = new TimescaleTier(),
    MiddleTimescaleTier = new TimescaleTier(),
    BottomTimescaleTier = new TimescaleTier()
};

// установить количество шкал времени
view.TopTimescaleTier.Count = 2;
view.TopTimescaleTier.Unit = TimescaleUnit.Quarters;
view.TopTimescaleTier.Label = DateLabel.QuarterQQyy;
view.TopTimescaleTier.ShowTicks = false;

view.MiddleTimescaleTier.Count = 2;
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
view.MiddleTimescaleTier.ShowTicks = false;

view.BottomTimescaleTier.Unit = TimescaleUnit.Days;
view.BottomTimescaleTier.Label = DateLabel.DayDdd;
view.BottomTimescaleTier.Count = 2;
view.BottomTimescaleTier.ShowTicks = false;

// добавить представление диаграммы Ганта в проект
project.Views.Add(view);

// добавить некоторые тестовые данные в проект
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

// Используйте параметр 'Timescale.DefinedInView' для отрисовки шкал времени с использованием настроек шкалы времени, которые мы задали (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView,
    StartDate = DateTime.Now.AddDays(-30),
    EndDate = DateTime.Now.AddDays(30)
};

project.Save(OutDir + "WorkWithTimescaleTier_out.pdf", pdfSaveOptions);
```

### См. также

* enum [Timescale](../../../aspose.tasks.visualization/timescale/)
* class [SaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../saveoptions/)
* assembly [Aspose.Tasks](../../../)


