---
title: "Класс HtmlSaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Saving.HtmlSaveOptions. Позволяет указывать дополнительные параметры при рендеринге страниц проекта в HTML"
type: docs
weight: 2010
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
| [HtmlSaveOptions](htmlsaveoptions/)() | Инициализирует новый экземпляр класса `HtmlSaveOptions`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Получает или задает список экземпляров класса [`BarStyle`](../../aspose.tasks.visualization/barstyle/), которые отображаются в представлении проекта. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/) { get; set; } | Получает или задает префикс CSS‑стилей. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Получает или задает дату завершения рендеринга. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss/) { get; set; } | Получает или задает способ экспорта CSS. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts/) { get; set; } | Получает или задает способ экспорта шрифтов. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages/) { get; set; } | Получает или задает способ экспорта изображений. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Получает или задает значение, указывающее, следует ли увеличивать высоту строки, чтобы она соответствовала содержимому. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Получает или задает типы гарнитур шрифтов. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения шрифта. |
| [FontSettings](../../aspose.tasks.saving/htmlsaveoptions/fontsettings/) { get; } | Указывает настройки шрифта, используемые при рендеринге представления проекта. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Получает или задает список [`Gridline`](../../aspose.tasks.visualization/gridline/), отображаемых в представлении проекта. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Получает или задает обратный вызов, который вызывается для создания ресурса для хранения шрифта. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/) { get; set; } | Получает или задает значение, указывающее, включать ли название проекта в заголовок HTML‑страницы. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/) { get; set; } | Получает или задает значение, указывающее, включать ли название проекта в заголовок HTML. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Получает или задает значение, определяющее, как отрисовывать легенду. Значение по умолчанию — LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Получает или задает массив PageLegendItem, определяющий, какие полосы должны отображаться в легенде страницы. Если null, отображаются элементы по умолчанию. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Получает или задает количество страниц проекта. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages/) { get; set; } | Получает или задает список номеров страниц для сохранения при рендеринге макета проекта. Если список пуст, будут сохранены все страницы проекта. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Получает или задает пользовательский обратный вызов, используемый для получения выходного потока для каждой отрисованной страницы. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Получает или задает размер страницы для рендеринга (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Получает или задает [`PresentationFormat`](../saveoptions/presentationformat/), в котором будет сохранён документ. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap/) { get; set; } | Получает или задает значение, указывающее, следует ли уменьшить зазор между последней задачей и нижним колонтитулом. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Получает или задает значение, указывающее, следует ли рендерить проект в одну страницу при сохранении проекта в графическом формате. Размер страницы будет изменён, чтобы отрисованный проект поместился на одной странице. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Получает или задает значение, указывающее, следует ли помечать подпроекты на полосе сводной задачи. Для подпроектов поле Rollup указывает, будет ли информация о ганттовых полосах подпроекта агрегирована в полосу сводной задачи. Для сводных задач поле Rollup указывает, отображает ли полоса сводной задачи агрегированные полосы. Для того чтобы любые подпроекты агрегировались, поле Rollup для сводных задач должно быть установлено в Yes. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Получает или задает дату, с которой начинается отрисовка. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки некоторых аспектов отрисовки связей задач. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Получает или задает список стилей текста, применяемых при отрисовке представления проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Получает или задает значение [`Timescale`](../saveoptions/timescale/), которое используется для управления тем, как отрисовывается шкала времени (если присутствует) при сохранении проекта в графическом формате. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Получает или задает поведение, определяющее, как выравнивать правый конец шкалы времени с концом страницы. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush/) { get; set; } | Получает или задает значение, указывающее, использовать ли градиентную кисть при отрисовке макета проекта. В настоящее время использование градиентной кисти не поддерживается при отрисовке в HTML. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Получает или задает список столбцов представления для отрисовки ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Если не задано, отрисовываются только идентификаторы задач, их имена, начало и окончание. Если заданы оба свойства View и [`ViewSettings`](../saveoptions/viewsettings/), столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Получает или задает представление ([`View`](../saveoptions/view/)) для отрисовки. Вы можете использовать эту опцию, чтобы явно указать, какое представление следует сохранять в форматы PDF, HTML или Image. Если это свойство задано, свойство [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) игнорируется при сохранении проекта. Представление должно быть одним из следующих экранов (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Примеры

Показывает, как сохранить проект в формате HTML.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var option = new HtmlSaveOptions();
project.Save(OutDir + "SaveProjectDataAsHTML_out.html", option);

// ИЛИ

// Добавление только одной страницы (страница номер 2).
option = new HtmlSaveOptions();
option.Pages.Add(2);
project.Save(OutDir + "SaveProjectDataAsHTML2_out.html", option);
```

### См. также

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


