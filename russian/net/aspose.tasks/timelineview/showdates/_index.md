---
title: "TimelineView.ShowDates"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство TimelineView. Возвращает значение, указывающее, показывать ли даты"
type: docs
weight: 40
url: /ru/net/aspose.tasks/timelineview/showdates/
---
## TimelineView.ShowDates property

Получает значение, указывающее, показывать ли даты.

```csharp
public bool ShowDates { get; }
```

## Примеры

Показывает, как работать с &lt;see cref="Aspose.Tasks.TimelineView" /&gt;.

```csharp
var project = new Project();

// инициализировать представление временной шкалы
var view = new TimelineView();

// задать значение, указывающее, как форматировать даты во view Timeline.
view.DateFormat = DateFormat.DateDddDd;
// задать значение, указывающее, отображать ли перекрывающиеся задачи в несколь­ких строках.
view.DisplayOverlapped = true;
// задать значение, указывающее, показывать ли элементы управления панорамированием и масштабированием.
view.ShowPanZoom = true;
// задать значение, указывающее, показывать ли шкалу времени.
view.ShowTimescale = true;
// задать значение, указывающее, отображать ли линию, представляющую текущий день.
view.ShowToday = true;
// задать значение, указывающее, сколько линий используется для отображения задач во временной шкале.
view.TextLinesCount = 2;

// получает значение, указывающее, отображать ли перекрывающиеся задачи в нескольких строках.
Console.WriteLine("Show Dates: " + view.ShowDates);

// добавить представление в проект
project.Views.Add(view);

// добавить некоторые тестовые данные в проект
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task1.Set(Tsk.Duration, task1.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 4, 29, 8, 0, 0));
task2.Set(Tsk.Duration, task1.ParentProject.GetDuration(40, TimeUnitType.Hour));

project.Save(OutDir + "SetTimeScaleCount_out.pdf", SaveFileFormat.Pdf);
```

### См. также

* class [TimelineView](../)
* namespace [Aspose.Tasks](../../timelineview/)
* assembly [Aspose.Tasks](../../../)


