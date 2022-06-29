---
title: CsvOptions
second_title: Справочник по Aspose.Tasks для .NET API
description: Позволяет указать дополнительные параметры при сохранении проекта в CSV.
type: docs
weight: 1710
url: /ru/net/aspose.tasks.saving/csvoptions/
---
## CsvOptions class

Позволяет указать дополнительные параметры при сохранении проекта в CSV.

```csharp
public class CsvOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CsvOptions](csvoptions)() | Инициализирует новый экземпляр класса[`CsvOptions`](../csvoptions), который можно использовать для сохранения проекта в формате CSV. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Получает или задает список экземпляров класса[`BarStyle`](../../aspose.tasks.visualization/barstyle), отображаемых в представлении проекта. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DataCategory](../../aspose.tasks.saving/csvoptions/datacategory) { get; set; } | Получает или задает категорию данных для сохранения. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [Encoding](../../aspose.tasks.saving/csvoptions/encoding) { get; set; } | Получает или задает кодировку для сохранения CSV. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Получает или задает дату окончания рендеринга. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Получает или задает значение, указывающее, следует ли увеличить высоту строки, чтобы она соответствовала ее содержимому. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Получает или задает список[`Gridline`](../../aspose.tasks.visualization/gridline), которые отображаются в представлении проекта. |
| [IncludeHeaders](../../aspose.tasks.saving/csvoptions/includeheaders) { get; set; } | Получает или задает значение, указывающее, следует ли включать заголовки или нет (значение по умолчанию — TRUE). |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Получает или задает значение, указывающее, следует ли отображать легенду на каждой странице (значение по умолчанию — TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Получает или задает количество страниц проекта. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Получает или задает размер отображаемой страницы (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Получает или задает[`PresentationFormat`](../saveoptions/presentationformat), в котором будет сохранен документ. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Получает или задает значение, указывающее, должен ли проект отображаться на одной странице при сохранении проекта в графическом формате. Размер страницы будет изменен, чтобы отрендеренный проект мог уместиться на одной странице. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Получает или задает значение, указывающее, следует ли помечать подзадачи на панели сводных задач. Для подзадач поле Свернуть указывает, будет ли информация на диаграммах Ганта для подзадач сворачиваться в панель сводных задач. Для сводных задач поле Сводка указывает, отображаются ли на панели сводных задач свернутые столбцы. В поле "Сводка" для сводных задач должно быть установлено значение "Да", чтобы к ним можно было сводить любые подзадачи. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Получает или задает формат, в котором будет сохранен документ, если используется этот объект параметров сохранения. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Получает или задает дату начала рендеринга. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и диаграмме листа задач. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Получает или задает условие, которое используется для фильтрации задач, отображаемых на диаграммах Ганта, листе задач и диаграммах использования задач. |
| [TextDelimiter](../../aspose.tasks.saving/csvoptions/textdelimiter) { get; set; } | Получает или задает разделитель текста. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Получает или задает список экземпляров класса[`TextStyle`](../../aspose.tasks.visualization/textstyle), отображаемых в представлении проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Получает или задает значение[`Timescale`](../saveoptions/timescale), которое используется для управления шкалой времени (если имеется) отображается при сохранении проекта в графическом формате. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Получает или задает значение, указывающее, следует ли использовать градиентную кисть при отображении диаграммы Ганта. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Получает или задает список столбцов представления для отображения ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)). Если не установлено, то отображаются только идентификаторы задач, имена задач, начало и конец. Если заданы свойства View и[`ViewSettings`](../saveoptions/viewsettings), столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Получает или задает представление ([`View`](../saveoptions/view)) для рендеринга. Вы можете использовать эти параметры, чтобы явно указать, какое представление должно быть сохранено в форматах PDF, HTML или изображения. Если установлено это свойство, свойство[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)игнорируется при сохранении проекта. Представление должно быть с одного из следующих экранов (([`Screen`](../../aspose.tasks/view/screen))):(Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
