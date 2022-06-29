---
title: GanttChartView
second_title: Справочник по Aspose.Tasks для .NET API
description: Представляет представление диаграммы Ганта.
type: docs
weight: 690
url: /ru/net/aspose.tasks/ganttchartview/
---
## GanttChartView class

Представляет представление диаграммы Ганта.

```csharp
public class GanttChartView : View
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GanttChartView](ganttchartview)() | Инициализирует новый экземпляр класса[`GanttChartView`](../ganttchartview). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoFilters](../../aspose.tasks/ganttchartview/autofilters) { get; } | Получает список автоматических фильтров представления диаграммы Ганта. |
| [BarRounding](../../aspose.tasks/ganttchartview/barrounding) { get; set; } | Получает или задает значение, указывающее, округляются ли столбцы до ближайшего дня. Значение по умолчанию — True. |
| [BarSize](../../aspose.tasks/ganttchartview/barsize) { get; set; } | Получает или задает высоту (в пунктах) столбцов Ганта на диаграмме Ганта. |
| [BarStyles](../../aspose.tasks/ganttchartview/barstyles) { get; } | Получает список родительских (общих) стилей столбцов представления диаграммы Ганта. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle). |
| [BottomTimescaleTier](../../aspose.tasks/ganttchartview/bottomtimescaletier) { get; set; } | Получает или задает настройки нижнего уровня временной шкалы представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier) |
| [CustomBarStyles](../../aspose.tasks/ganttchartview/custombarstyles) { get; } | Получает список настраиваемых стилей столбцов для конкретных задач в представлении диаграммы Ганта. [`GanttBarStyle`](../../aspose.tasks.visualization/ganttbarstyle). |
| [Filter](../../aspose.tasks/view/filter) { get; set; } | Получает или задает фильтр, используемый в одном представлении. |
| [Gridlines](../../aspose.tasks/ganttchartview/gridlines) { get; set; } | Получает или задает список[`Gridlines`](./gridlines)представления диаграммы Ганта. |
| [Group](../../aspose.tasks/view/group) { get; set; } | Получает или задает группу одного представления. |
| [HideRollupBarsWhenSummaryExpanded](../../aspose.tasks/ganttchartview/hiderollupbarswhensummaryexpanded) { get; set; } | Получает или задает значение, указывающее, будут ли панели сводки скрыты при развертывании сводной задачи. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter) { get; set; } | Получает или задает значение, указывающее, выделяет ли Microsoft Project фильтр для одного представления. |
| [MiddleTimescaleTier](../../aspose.tasks/ganttchartview/middletimescaletier) { get; set; } | Получает или задает настройки среднего уровня шкалы времени представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier). |
| [Name](../../aspose.tasks/view/name) { get; set; } | Получает или задает имя объекта View. |
| [NonWorkingTimeColor](../../aspose.tasks/ganttchartview/nonworkingtimecolor) { get; set; } | Получает или устанавливает цвет нерабочего времени. |
| [PageInfo](../../aspose.tasks/view/pageinfo) { get; } | Получает экземпляр класса[`PageInfo`](../view/pageinfo). Представляет данные настройки страницы, представленные в формате файла mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject) { get; } | Получает родителя объекта View. Только чтение[`Project`](../project). |
| [ProgressLines](../../aspose.tasks/ganttchartview/progresslines) { get; set; } | Получает или задает линии прогресса для представления диаграммы Ганта. [`ProgressLines`](./progresslines). |
| [RollUpGanttBars](../../aspose.tasks/ganttchartview/rollupganttbars) { get; set; } | Получает или задает значение, указывающее, должны ли столбцы на диаграмме Ганта сворачиваться. |
| [Screen](../../aspose.tasks/view/screen) { get; } | Получает тип экрана для одиночного представления. Только для чтения[`ViewScreen`](../viewscreen). |
| [ShowBarSplits](../../aspose.tasks/ganttchartview/showbarsplits) { get; set; } | Получает или задает значение, указывающее, должны ли отображаться разбиения задач на диаграмме Ганта. |
| [ShowDrawings](../../aspose.tasks/ganttchartview/showdrawings) { get; set; } | Получает или задает значение, указывающее, должны ли отображаться рисунки на диаграмме Ганта. |
| [ShowInMenu](../../aspose.tasks/view/showinmenu) { get; set; } | Получает или задает значение, указывающее, показывает ли Microsoft Project одно имя представления в раскрывающихся списках Представление или Другие представления на ленте. |
| [Table](../../aspose.tasks/view/table) { get; set; } | Получает или задает таблицу одного представления. |
| [TableTextStyles](../../aspose.tasks/ganttchartview/tabletextstyles) { get; } | Получает список стилей текста таблицы представления диаграммы Ганта. [`TableTextStyle`](../../aspose.tasks.visualization/tabletextstyle). |
| [TextStyles](../../aspose.tasks/ganttchartview/textstyles) { get; set; } | Получает или задает список[`TextStyle`](../../aspose.tasks.visualization/textstyle)представления диаграммы Ганта. |
| [TimescaleSizePercentage](../../aspose.tasks/ganttchartview/timescalesizepercentage) { get; set; } |  |
| [TopTimescaleTier](../../aspose.tasks/ganttchartview/toptimescaletier) { get; set; } | Получает или задает настройки верхнего уровня временной шкалы представления. [`TimescaleTier`](../../aspose.tasks.visualization/timescaletier). |
| [Type](../../aspose.tasks/view/type) { get; } | Получает тип элемента в отдельном представлении, например задачи или ресурсы. Только для чтения[`ItemType`](../itemtype). |
| [Uid](../../aspose.tasks/view/uid) { get; } | Получает уникальный идентификатор представления. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements) { get; } | Получает коллекцию объектов, представляющих размещение и внешний вид[`OleObject`](../oleobject)в представлении. |

## Методы

| Имя | Описание |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto)(View) | Сравнивает текущий экземпляр с другим объектом того же типа и возвращает целое число, указывающее, предшествует ли текущий экземпляр, следует за ним или находится в той же позиции в порядке сортировки как другой объект. |
| override [Equals](../../aspose.tasks/view/equals)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode)() | Возвращает значение хэш-кода для экземпляра класса[`Resource`](../resource). |

### Смотрите также

* class [View](../view)
* пространство имен [Aspose.Tasks](../../aspose.tasks)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
