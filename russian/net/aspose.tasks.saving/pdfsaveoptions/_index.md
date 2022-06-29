---
title: PdfSaveOptions
second_title: Справочник по Aspose.Tasks для .NET API
description: Позволяет указать дополнительные параметры при рендеринге страниц проекта в PDF.
type: docs
weight: 1850
url: /ru/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Позволяет указать дополнительные параметры при рендеринге страниц проекта в PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions)() | Инициализирует новый экземпляр класса[`PdfSaveOptions`](../pdfsaveoptions), который можно использовать для сохранения документа в[`Формат PDF`](../savefileformat) . |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Получает или задает список экземпляров класса[`BarStyle`](../../aspose.tasks.visualization/barstyle), отображаемых в представлении проекта. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance) { get; set; } | Получает или задает желаемый уровень соответствия для сгенерированного PDF-документа. По умолчанию:Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Получает или задает пользовательский размер страницы в пунктах (1 пункт = 1/72 дюйма). |
| [DefaultFontName](../../aspose.tasks.saving/pdfsaveoptions/defaultfontname) { get; set; } | Получает или задает шрифт по умолчанию для визуализации. |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails) { get; set; } | Получает или задает сведения о цифровой подписи. Если не задано, то подписание производиться не будет. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Получает или задает значение, указывающее, следует ли отображать нерабочее время (значение по умолчанию — TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails) { get; set; } | Получает или устанавливает детали шифрования. Если не установлено, то шифрование выполняться не будет. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Получает или задает дату окончания рендеринга. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Получает или задает значение, указывающее, следует ли увеличить высоту строки, чтобы она соответствовала ее содержимому. |
| [FontResolveCallback](../../aspose.tasks.saving/pdfsaveoptions/fontresolvecallback) { get; set; } | Получает или задает обратный вызов, который можно использовать для настройки разрешенных шрифтов. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Получает или задает список[`Gridline`](../../aspose.tasks.visualization/gridline), которые отображаются в представлении проекта. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Получает или задает значение, указывающее, следует ли отображать легенду на каждой странице (значение по умолчанию — TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Получает или задает значение, указывающее, должны ли критические задачи отображаться красным цветом (значение по умолчанию — FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Получает или задает цвет нерабочего времени. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Получает или задает количество страниц проекта. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages) { get; set; } | Получает или задает список номеров страниц для сохранения при сохранении макета проекта в отдельные файлы.  Все страницы будут сохранены, если этот список пуст. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback) { get; set; } | Получает или задает определяемый пользователем обратный вызов, который используется для получения выходного потока для каждой отображаемой страницы. Применяется, когда используется опция[`SaveToSeparateFiles`](./savetoseparatefiles). |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Получает или задает размер отображаемой страницы (значение по умолчанию — PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Получает или задает[`PresentationFormat`](../saveoptions/presentationformat), в котором будет сохранен документ. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap) { get; set; } | Получает или задает значение, указывающее, должен ли быть уменьшен разрыв между последней задачей и нижним колонтитулом. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Получает или задает значение, указывающее, должен ли проект отображаться на одной странице при сохранении проекта в графическом формате. Размер страницы будет изменен, чтобы отрендеренный проект мог уместиться на одной странице. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Получает или задает значение, указывающее, следует ли помечать подзадачи на панели сводных задач. Для подзадач поле Свернуть указывает, будет ли информация на диаграммах Ганта для подзадач сворачиваться в панель сводных задач. Для сводных задач поле Сводка указывает, отображаются ли на панели сводных задач свернутые столбцы. В поле "Сводка" для сводных задач должно быть установлено значение "Да", чтобы к ним можно было сводить любые подзадачи. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Получает или задает формат, в котором будет сохранен документ, если используется этот объект параметров сохранения. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles) { get; set; } | Получает или задает значение, указывающее, следует ли сохранять страницы проекта в отдельные файлы. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Получает или задает дату начала рендеринга. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Получает или задает компаратор для сортировки задач на диаграмме Ганта и диаграмме листа задач. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Получает или задает условие, которое используется для фильтрации задач, отображаемых на диаграммах Ганта, листе задач и диаграммах использования задач. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression) { get; set; } | Получает или задает тип сжатия для всех потоков содержимого, кроме изображений. По умолчанию:Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Получает или задает список экземпляров класса[`TextStyle`](../../aspose.tasks.visualization/textstyle), отображаемых в представлении проекта. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Получает или задает значение[`Timescale`](../saveoptions/timescale), которое используется для управления шкалой времени (если имеется) отображается при сохранении проекта в графическом формате. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Получает или задает значение, указывающее, следует ли использовать градиентную кисть при отображении диаграммы Ганта. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/pdfsaveoptions/useprojectdefaultfont) { get; set; } | Получает или задает значение, указывающее, должен ли использоваться шрифт по умолчанию для визуализации. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Получает или задает список столбцов представления для отображения ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn)). Если не установлено, то отображаются только идентификаторы задач, имена задач, начало и конец. Если заданы свойства View и[`ViewSettings`](../saveoptions/viewsettings), столбцы из View переопределяют столбцы из ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Получает или задает представление ([`View`](../saveoptions/view)) для рендеринга. Вы можете использовать эти параметры, чтобы явно указать, какое представление должно быть сохранено в форматах PDF, HTML или изображения. Если установлено это свойство, свойство[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)игнорируется при сохранении проекта. Представление должно быть с одного из следующих экранов (([`Screen`](../../aspose.tasks/view/screen))):(Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
