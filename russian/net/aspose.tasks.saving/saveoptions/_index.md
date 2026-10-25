---
title: "Класс SaveOptions"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.SaveOptions класс. Это абстрактный базовый класс для классов, позволяющих пользователю указывать дополнительные параметры при сохранении проекта в определённый формат."
type: docs
weight: 2190
url: /ru/net/aspose.tasks.saving/saveoptions/
---
## SaveOptions class

Это абстрактный базовый класс для классов, позволяющих пользователю указывать дополнительные параметры при сохранении проекта в определённый формат.

```csharp
public abstract class SaveOptions : SimpleSaveOptions
```

## Свойства

| Имя | Описание |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Получает или задает список экземпляров класса [`BarStyle`](../../aspose.tasks.visualization/barstyle/), которые отображаются в представлении проекта. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Получает или задает дату завершения рендеринга. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Получает или задает значение, указывающее, следует ли увеличивать высоту строки, чтобы она соответствовала содержимому. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Получает или задает список [`Gridline`](../../aspose.tasks.visualization/gridline/), отображаемых в представлении проекта. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Получает или задает значение, указывающее, является ли ориентация страницы портретной; возвращает false, если ориентация страницы альбомная. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Получает или задает значение, определяющее, как отрисовывать легенду. Значение по умолчанию — LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Получает или задает массив PageLegendItem, определяющий, какие полосы должны отображаться в легенде страницы. Если null, отображаются элементы по умолчанию. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Получает или задает количество страниц проекта. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Получает или задает размер страницы для рендеринга (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Получает или задает [`PresentationFormat`](./presentationformat/), в котором будет сохранён документ. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Получает или задает значение, указывающее, следует ли рендерить проект в одну страницу при сохранении проекта в графическом формате. Размер страницы будет изменён, чтобы отрисованный проект поместился на одной странице. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Получает или задает значение, указывающее, следует ли помечать подпроекты на полосе сводной задачи. Для подпроектов поле Rollup указывает, будет ли информация о ганттовых полосах подпроекта агрегирована в полосу сводной задачи. Для сводных задач поле Rollup указывает, отображает ли полоса сводной задачи агрегированные полосы. Для того чтобы любые подпроекты агрегировались, поле Rollup для сводных задач должно быть установлено в Yes. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Получает или задает формат, в котором будет сохраняться документ, если используется этот объект параметров сохранения. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Получает или задает дату, с которой начинается отрисовка. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки некоторых аспектов отрисовки связей задач. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и листе задач. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Получает или задает условие, используемое для фильтрации задач, отрисованных на диаграммах Ганта, листе задач и использовании задач. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Получает или задает список стилей текста, применяемых при отрисовке представления проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Получает или задает значение [`Timescale`](./timescale/), которое используется для управления тем, как отображается шкала времени (если присутствует) при сохранении проекта в графическом формате. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Получает или задает поведение, определяющее, как выравнивать правый конец шкалы времени с концом страницы. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Получает или задает значение, указывающее, следует ли использовать градиентную кисть при рендеринге диаграммы Ганта. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Получает или задает список столбцов представления для отображения ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Если не задано, отображаются только идентификаторы задач, названия задач, даты начала и окончания. Если заданы оба свойства View и [`ViewSettings`](./viewsettings/), столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Получает или задает представление ([`View`](./view/)) для рендеринга. Вы можете использовать эту опцию, чтобы явно указать, какое представление следует сохранять в форматы PDF, HTML или Image. Если это свойство задано, свойство [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) игнорируется при сохранении проекта. Представление должно быть выбрано из одного из следующих экранов (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

## Примечания

Экземпляр любого производного класса от класса SaveOptions передаётся в перегрузки Save для потока или строки, чтобы пользователь мог определить пользовательские параметры при сохранении документа.

## Примеры

Показывает, как установить параметр, увеличивать ли высоту строки, чтобы она соответствовала содержимому.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
SaveOptions options = new PdfSaveOptions
{
    // Установить параметр fit content в значение true
    FitContent = true,
    Timescale = Timescale.Months,
    PresentationFormat = PresentationFormat.TaskUsage
};
project.Save(OutDir + "FitContentsToCellSize_out.pdf", options);
```

### См. также

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


