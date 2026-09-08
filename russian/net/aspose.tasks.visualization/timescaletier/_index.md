---
title: "Класс TimescaleTier"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Visualization.TimescaleTier. Представляет отдельный уровень шкалы времени на диаграмме Ганта"
type: docs
weight: 3450
url: /ru/net/aspose.tasks.visualization/timescaletier/
---
## TimescaleTier class

Представляет один уровень шкалы времени на диаграмме Ганта.

```csharp
public sealed class TimescaleTier
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TimescaleTier](timescaletier/#constructor)() | Инициализирует новый экземпляр класса `TimescaleTier`. |
| [TimescaleTier](timescaletier/#constructor_1)(TimescaleUnit, int) | Инициализирует новый экземпляр класса `TimescaleTier`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Alignment](../../aspose.tasks.visualization/timescaletier/alignment/) { get; set; } | Получает или задает способ выравнивания меток внутри каждого временного периода уровня ([`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [Count](../../aspose.tasks.visualization/timescaletier/count/) { get; set; } | Получает или задает интервал единицы времени, в котором отображаются метки уровня. Значение по умолчанию — 1. |
| [DateTimeConverter](../../aspose.tasks.visualization/timescaletier/datetimeconverter/) { get; set; } | Получает или задает функцию обратного вызова для обработки отрисовки отметки даты в этом уровне. |
| [Label](../../aspose.tasks.visualization/timescaletier/label/) { get; set; } | Получает или задает метку даты [`DateLabel`](../datelabel/) для уровня шкалы времени. |
| [RenderLabelOnEachPage](../../aspose.tasks.visualization/timescaletier/renderlabeloneachpage/) { get; set; } | Получает или задает флаг, определяющий, следует ли отображать метки даты на каждой странице, когда временной период охватывает несколько страниц. Если значение 'true', при охвате периода несколькими страницами метки даты для периода отображаются на каждой странице. Если значение 'false', метка даты отображается только один раз в соответствии со значением свойства [`Alignment`](./alignment/). |
| [ShowTicks](../../aspose.tasks.visualization/timescaletier/showticks/) { get; set; } | Получает или задает значение, указывающее, показывать ли отметки, разделяющие временные периоды в уровне. |
| [Unit](../../aspose.tasks.visualization/timescaletier/unit/) { get; set; } | Получает или задает единицу шкалы времени [`TimescaleUnit`](../timescaleunit/) для уровня шкалы времени. Значение по умолчанию — [`Days`](../timescaleunit/). |
| [UsesFiscalYear](../../aspose.tasks.visualization/timescaletier/usesfiscalyear/) { get; set; } | Получает или задает значение, указывающее, основывать ли метки уровня на финансовом году. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


