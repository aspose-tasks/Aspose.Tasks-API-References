---
title: "TimescaleTier.UsesFiscalYear"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TimescaleTier. Получает или задает значение, указывающее, следует ли основывать метки уровня на финансовом году."
type: docs
weight: 90
url: /ru/net/aspose.tasks.visualization/timescaletier/usesfiscalyear/
---
## TimescaleTier.UsesFiscalYear property

Получает или задает значение, указывающее, основывать ли метки уровня на финансовом году.

```csharp
public bool UsesFiscalYear { get; set; }
```

## Примеры

Показывает, как настроить метки уровня шкалы времени.

```csharp
var project = new Project(DataDir + "CreateProject1.mpp");

// Добавить ссылки на задачи
project.TaskLinks.Add(project.RootTask.Children.Add("Task 1"), project.RootTask.Children.Add("Task 2"));

var view = (GanttChartView)project.DefaultView;

// настроить уровни шкалы времени

// настроить верхний уровень
// установить верхний уровень шкалы времени представления диаграммы Ганта.
view.MiddleTimescaleTier = new TimescaleTier();
// установить единицу шкалы времени <see cref="T:Aspose.Tasks.Visualization.TimescaleUnit" /> для уровня шкалы времени.
view.MiddleTimescaleTier.Unit = TimescaleUnit.Weeks;
// установить интервал единицы времени, в котором отображаются метки уровня.
view.MiddleTimescaleTier.Count = 1;
// установить метку даты <see cref="T:Aspose.Tasks.Visualization.DateLabel" /> для уровня шкалы времени.
view.MiddleTimescaleTier.Label = DateLabel.WeekDddDd;
// установить способ выравнивания меток внутри каждого временного периода уровня (<see cref="T:System.Drawing.StringAlignment" />).
view.MiddleTimescaleTier.Alignment = HorizontalStringAlignment.Center;
// установить значение, указывающее, следует ли показывать метки деления, разделяющие временные периоды в уровне.
view.MiddleTimescaleTier.ShowTicks = true;
// установить значение, указывающее, следует ли основывать подписи уровней на финансовом году.
view.MiddleTimescaleTier.UsesFiscalYear = true;

// добавлено для лучшей визуализации
view.TopTimescaleTier = new TimescaleTier(TimescaleUnit.Months, 1);

// настроить даты среднего уровня
view.TopTimescaleTier.DateTimeConverter = date =>
    new[] { "Янв.", "Фев.", "Мар.", "Апр.", "Май", "Июнь", "Июль", "Авг.", "Сен.", "Окт.", "Ноя.", "Дек." }[date.Month - 1];

project.Set(Prj.TimescaleStart, new DateTime(2012, 7, 30));
project.Set(Prj.TimescaleFinish, new DateTime(2012, 10, 6));

// Используйте параметр 'Timescale.DefinedInView' для отображения шкал времени с использованием настроек шкалы, определённых во view (view.TopTimescaleTier, view.MiddleTimescaleTier, view.BottomTimescaleTier).
var pdfSaveOptions = new PdfSaveOptions
{
    Timescale = Timescale.DefinedInView
};

project.Save(OutDir + "CustomizeTimescaleTierLabels_out.pdf", pdfSaveOptions);
```

### См. также

* class [TimescaleTier](../)
* namespace [Aspose.Tasks.Visualization](../../timescaletier/)
* assembly [Aspose.Tasks](../../../)


