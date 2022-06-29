---
title: HtmlSaveOptions
second_title: Справочник по Aspose.Tasks для .NET API
description: Позволяет указать дополнительные параметры при рендеринге страниц проекта в HTML.
type: docs
weight: 1740
url: /ru/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Позволяет указать дополнительные параметры при рендеринге страниц проекта в HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions)() | Инициализирует новый экземпляр класса[`HtmlSaveOptions`](../htmlsaveoptions). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Получает или задает список экземпляров класса[`BarStyle`](../../aspose.tasks.visualization/barstyle), отображаемых в представлении проекта. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix) { get; set; } | Получает или задает префикс стиля CSS. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DefaultFontName](../../aspose.tasks.saving/htmlsaveoptions/defaultfontname) { get; set; } | Получает или задает шрифт по умолчанию для визуализации. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Получает или задает дату окончания рендеринга. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss) { get; set; } | Получает или задает способ экспорта CSS. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts) { get; set; } | Получает или задает способ экспорта шрифтов. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages) { get; set; } | Получает или задает способ экспорта изображений. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Получает или задает значение, указывающее, следует ли увеличить высоту строки, чтобы она соответствовала ее содержимому. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes) { get; set; } | Получает или задает типы шрифта. |
| [FontResolveCallback](../../aspose.tasks.saving/htmlsaveoptions/fontresolvecallback) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки разрешенных шрифтов. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения шрифта. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Получает или задает список[`Gridline`](../../aspose.tasks.visualization/gridline), которые отображаются в представлении проекта. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения шрифта. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader) { get; set; } | Получает или задает значение, указывающее, следует ли включать имя проекта в заголовок HTML-страницы. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle) { get; set; } | Получает или задает значение, указывающее, следует ли включать имя проекта в заголовок HTML. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Получает или задает значение, указывающее, следует ли отображать легенду на каждой странице (значение по умолчанию — TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Получает или задает количество страниц проекта. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages) { get; set; } | Получает или задает список номеров страниц для сохранения при отрисовке макета проекта.  Все страницы проекта будут сохранены, если этот список пуст. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback) { get; set; } | Получает или задает определяемый пользователем обратный вызов, который используется для получения выходного потока для каждой отображаемой страницы. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Получает или задает размер отображаемой страницы (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Получает или задает[`PresentationFormat`](../saveoptions/presentationformat), в котором будет сохранен документ. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap) { get; set; } | Получает или задает значение, указывающее, должен ли быть уменьшен разрыв между последней задачей и нижним колонтитулом. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Получает или задает значение, указывающее, должен ли проект отображаться на одной странице при сохранении проекта в графическом формате. Размер страницы будет изменен, чтобы отрендеренный проект мог уместиться на одной странице. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Получает или задает значение, указывающее, следует ли помечать подзадачи на панели сводных задач. Для подзадач поле Свернуть указывает, будет ли информация на диаграммах Ганта для подзадач сворачиваться в панель сводных задач. Для сводных задач поле Сводка указывает, отображаются ли на панели сводных задач свернутые столбцы. В поле "Сводка" для сводных задач должно быть установлено значение "Да", чтобы к ним можно было сводить любые подзадачи. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Получает или задает формат, в котором будет сохранен документ, если используется этот объект параметров сохранения. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Получает или задает дату начала рендеринга. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и диаграмме листа задач. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Получает или задает условие, которое используется для фильтрации задач, отображаемых на диаграммах Ганта, листе задач и диаграммах использования задач. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Получает или задает список экземпляров класса[`TextStyle`](../../aspose.tasks.visualization/textstyle), отображаемых в представлении проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Получает или задает значение[`Timescale`](../saveoptions/timescale), которое используется для управления шкалой времени (если имеется) отображается при сохранении проекта в графическом формате. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush) { get; set; } | Получает или задает значение, указывающее, следует ли использовать градиентную кисть при отрисовке макета проекта.  В настоящее время использование градиентной кисти не поддерживается при рендеринге в HTML. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont) { get; set; } | Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для визуализации. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Получает или задает список столбцов представления для отображения ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)). Если не установлено, то отображаются только идентификаторы задач, имена задач, начало и конец. Если заданы свойства View и[`ViewSettings`](../saveoptions/viewsettings), столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Получает или задает представление ([`View`](../saveoptions/view)) для рендеринга. Вы можете использовать эти параметры, чтобы явно указать, какое представление должно быть сохранено в форматах PDF, HTML или изображения. Если установлено это свойство, свойство[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)игнорируется при сохранении проекта. Представление должно быть с одного из следующих экранов (([`Screen`](../../aspose.tasks/view/screen))):(Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
