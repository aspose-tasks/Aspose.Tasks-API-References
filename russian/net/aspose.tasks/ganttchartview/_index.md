---
title: "Класс GanttChartView"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GanttChartView. Представляет представление GanttChart."
type: docs
weight: 710
url: /ru/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Представляет представление GanttChart.

```csharp
public class GanttChartView : View
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GanttChartView](ganttchartview/)() | Инициализирует новый экземпляр класса `GanttChartView`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters/) { get; } | Получает список автофильтров представления диаграммы Ганта. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding/) { get; set; } | Получает или задает значение, указывающее, округляются ли полосы до ближайшего дня. Значение по умолчанию: True. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize/) { get; set; } | Получает или задает высоту, в пунктах, полос диаграммы Ганта. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles/) { get; } | Получает список стилей родительских (общих) полос представления диаграммы Ганта. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier/) { get; set; } | Получает или задает настройки нижнего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles/) { get; } | Получает список пользовательских стилей полос, специфичных для задач, представления диаграммы Ганта. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle/). |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Получает или задает фильтр, используемый в отдельном представлении. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines/) { get; set; } | Получает или задает список [`Gridlines`](./gridlines/) представления диаграммы Ганта. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Получает или задает группу отдельного представления. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded/) { get; set; } | Получает или задает значение, указывающее, будут ли скрыты сводные полосы при раскрытии сводной задачи. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для отдельного представления. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier/) { get; set; } | Получает или задает настройки среднего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Получает или задает имя объекта View. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor/) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Получает экземпляр класса [`PageInfo`](../view/pageinfo/). Представляет данные настройки страницы, присутствующие в формате файла mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Получает родителя объекта View. Только для чтения [`Project`](../project/). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines/) { get; set; } | Получает или задает линии прогресса для представления диаграммы Ганта. [`ProgressLines`](./progresslines/). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars/) { get; set; } | Получает или задает значение, указывающее, должны ли полосы на диаграмме Ганта быть свернуты. |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Получает тип экрана для отдельного представления. Только для чтения [`ViewScreen`](../viewscreen/). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits/) { get; set; } | Получает или задает значение, указывающее, должны ли отображаться разрывы задач на диаграмме Ганта. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings/) { get; set; } | Получает или задает значение, указывающее, должны ли отображаться рисунки на диаграмме Ганта. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Получает или задает значение, указывающее, отображает ли Microsoft Project имя отдельного представления в выпадающих списках View или Other Views на ленте. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Получает или задает таблицу отдельного представления. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles/) { get; } | Получает список стилей текста таблицы представления диаграммы Ганта. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle/). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles/) { get; set; } | Получает или задает список [`TextStyle`](../../aspose.tasks.visualization/textstyle/) представления диаграммы Ганта. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage/) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier/) { get; set; } | Получает или задает настройки верхнего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier/). |
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

* class [View](../view/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


