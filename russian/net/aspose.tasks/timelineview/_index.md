---
title: "Класс TimelineView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.TimelineView. Представляет представление временной шкалы проекта"
type: docs
weight: 2580
url: /ru/net/aspose.tasks/timelineview/
---
## TimelineView class

Представляет временную шкалу проекта.

```csharp
public class TimelineView : View
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TimelineView](timelineview/)() | Инициализирует новый экземпляр класса `TimelineView`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DateFormat](../../aspose.tasks/timelineview/dateformat/) { get; set; } | Получает или задает значение, указывающее, как форматировать даты во view Timeline. |
| [DisplayOverlapped](../../aspose.tasks/timelineview/displayoverlapped/) { get; set; } | Получает или задает значение, указывающее, отображать ли перекрывающиеся задачи в нескольких строках. |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Получает или задает фильтр, используемый в отдельном представлении. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Получает или задает группу отдельного представления. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Получает или задает имя объекта View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Получает экземпляр класса [`PageInfo`](../view/pageinfo/). Представляет данные настройки страницы, присутствующие в формате файла mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Получает родителя объекта View. Только для чтения [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Получает тип экрана для отдельного представления. Только для чтения [`ViewScreen`](../viewscreen/). |
| [ShowDates](../../aspose.tasks/timelineview/showdates/) { get; } | Получает значение, указывающее, показывать ли даты. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли Microsoft Project имя отдельного представления в выпадающих списках View или Other Views на ленте. |
| [ShowPanZoom](../../aspose.tasks/timelineview/showpanzoom/) { get; set; } | Получает или задает значение, указывающее, показывать ли элементы управления панорамированием и масштабированием. |
| [ShowTimescale](../../aspose.tasks/timelineview/showtimescale/) { get; set; } | Получает или задает значение, указывающее, показывать ли шкалу времени. |
| [ShowToday](../../aspose.tasks/timelineview/showtoday/) { get; set; } | Получает или задает значение, указывающее, отображать ли линию, представляющую текущий день. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Получает или задает таблицу отдельного представления. |
| [TextLinesCount](../../aspose.tasks/timelineview/textlinescount/) { get; set; } | Получает или задает значение, указывающее, сколько линий используется для отображения задач во временной шкале. |
| [Type](../../aspose.tasks/view/type/) { get; } | Получает тип элемента в отдельном представлении, например задачи или ресурсы. Только для чтения [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Получает уникальный идентификатор представления. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Получает коллекцию объектов, представляющих размещение и внешний вид [`OleObject`](../oleobject/) в представлении. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует за ним или находится в том же положении в порядке сортировки, что и другой объект. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Возвращает значение хеш-кода для экземпляра класса [`Resource`](../resource/). |

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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


