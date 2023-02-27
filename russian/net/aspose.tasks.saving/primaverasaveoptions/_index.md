---
title: Class PrimaveraSaveOptions
second_title: Справочник по Aspose.Tasks для .NET API
description: Aspose.Tasks.Saving.PrimaveraSaveOptions сорт. Позволяет указать дополнительные параметры при сохранении проекта в формате Primavera XER.
type: docs
weight: 1880
url: /ru/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Позволяет указать дополнительные параметры при сохранении проекта в формате Primavera XER.

```csharp
public class PrimaveraSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Инициализирует новый экземпляр`PrimaveraSaveOptions` класс. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Получает или задает приращение, используемое при перенумерации идентификаторов действий. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Получает или задает префикс, используемый при перенумерации идентификаторов действий. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Получает или задает суффикс, используемый при перенумерации идентификаторов действий. |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Получает или задает список экземпляров[`BarStyle`](../../aspose.tasks.visualization/barstyle/) класс, который отображается в представлении проекта. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Получает или задает дату завершения рендеринга. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Получает или задает значение, указывающее, следует ли увеличить высоту строки, чтобы она соответствовала ее содержимому. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Получает или задает, должен ли раздел календаря представления отображаться до конца (справа) последней страницы. Если значение равно false, раздел календаря отображается точно до EndDate, даже если на странице есть пустое место. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Получает или задает список[`Gridline`](../../aspose.tasks.visualization/gridline/) которые отображаются в представлении проекта. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать легенду на каждой странице (значение по умолчанию — TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Получает или задает количество страниц проекта. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Получает или задает размер отображаемой страницы (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Получает или задает[`PresentationFormat`](../saveoptions/presentationformat/) в котором документ будет сохранен. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Получает или задает значение, указывающее, должен ли проект отображаться на одной странице при сохранении проекта в графическом формате. Размер страницы будет изменен, чтобы отображаемый проект мог уместиться на одной странице. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Получает или задает значение, указывающее, нужно ли перенумеровывать идентификаторы действий. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Получает или задает значение, указывающее, должны ли быть отмечены подзадачи на панели сводных задач. Поле указывает, отображаются ли на панели сводных задач свернутые столбцы. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохранен документ, если используется этот объект параметров сохранения. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Получает или задает дату начала рендеринга. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и диаграмме листа задач. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Получает или задает условие, которое используется для фильтрации задач, отображаемых на диаграммах Ганта, листе задач и диаграммах использования задач. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Получает или задает список экземпляров[`TextStyle`](../../aspose.tasks.visualization/textstyle/) класс, который отображается в представлении проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Получает или задает[`Timescale`](../saveoptions/timescale/) значение, которое используется для управления визуализацией временной шкалы (если она присутствует) при сохранении проекта в графическом формате. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Получает или задает значение, указывающее, следует ли использовать градиентную кисть при визуализации диаграммы Ганта. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Получает или задает список столбцов представления для отображения ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). Если не задано, то визуализируются только идентификаторы задач, имена задач, начало и конец.[`ViewSettings`](../saveoptions/viewsettings/)свойства установлены, столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Получает или задает представление ([`View`](../saveoptions/view/) ) для рендеринга. Вы можете использовать эти параметры, чтобы явно указать, какое представление должно быть сохранено в форматах PDF, HTML или Image. Если это свойство установлено,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) свойство игнорируется при сохранении проекта. Вид должен быть на одном из следующих экранов (([`Screen`](../../aspose.tasks/view/screen/) )): (Ганта, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Смотрите также

* class [SaveOptions](../saveoptions/)
* пространство имен [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* сборка [Aspose.Tasks](../../)


