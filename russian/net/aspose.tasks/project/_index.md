---
title: Project
second_title: Справочник по Aspose.Tasks для .NET API
description: Представляет проект.
type: docs
weight: 1180
url: /ru/net/aspose.tasks/project/
---
## Project class

Представляет проект.

```csharp
public class Project
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Project](project#constructor)() | Инициализирует новый экземпляр класса[`Project`](../project). |
| [Project](project#constructor_1)(DbSettings) | Инициализирует новый экземпляр класса[`Project`](../project)для чтения данных из базы данных, которая указана экземпляром класс[`DbSettings`](../../aspose.tasks.connectivity/dbsettings). |
| [Project](project#constructor_2)(Stream) | Инициализирует новый экземпляр класса[`Project`](../project)из потока. |
| [Project](project#constructor_9)(StreamReader) | Инициализирует новый экземпляр класса[`Project`](../project)из экземпляра StreamReader. |
| [Project](project#constructor_10)(string) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл mpp или mpt). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Инициализирует новый экземпляр класса[`Project`](../project)из Stream с указанным экземпляр класса[`LoadOptions`](../loadoptions). |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл mpp или mpt). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Инициализирует новый экземпляр класса[`Project`](../project)из Stream с указанным экземпляр класса[`PrimaveraReadOptions`](../primaverareadoptions). |
| [Project](project#constructor_8)(Stream, string) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл mpp или mpt). |
| [Project](project#constructor_11)(string, LoadOptions) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл mpp или mpt) с указанным экземпляром класса[`LoadOptions`](../loadoptions). |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл mpp или mpt). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Инициализирует новый экземпляр класса[`Project`](../project)из шаблона (существующий файл MPP или MPT) с указанным экземпляром класса[`PrimaveraReadOptions`](../primaverareadoptions). |
| [Project](project#constructor_16)(string, string) | Инициализирует новый экземпляр класса[`Project`](../project)из защищенного паролем шаблона (существующий файл mpp или mpt). |

## Характеристики

| Имя | Описание |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Получает коллекцию встроенных свойств проекта. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Получает или устанавливает режим расчета проекта. Может быть одним из значений перечисления[`CalculationMode`](./calculationmode). |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Получает[`CalendarCollection`](../calendarcollection)объект этого экземпляра проекта. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Получает коллекцию, содержащую список критических задач, составляющих критический путь данного проекта.  Это операция O(n), где n — количество задач в проекте. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Получает коллекцию пользовательских свойств проекта. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Получает или задает представление проекта по умолчанию. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Получает экземпляр класса[`WeekDayCollection`](../weekdaycollection), который представляет набор рабочих дней и рабочего времени по умолчанию для проекта. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Получает экземпляр класса[`ProjectDisplayOptions`](../projectdisplayoptions). |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Получает объект ExtendedAttributeDefinitionCollection. Набор определений расширенных атрибутов (настраиваемых полей), связанных с проектом. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Получает коллекцию, содержащую экземпляры класса[`OleObject`](../oleobject), которые связаны или внедрены в этот файл проекта.  Доступно только для файлов формата mpp. Эта коллекция доступна только для чтения, за исключением операции «Очистить». |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Получает объект OutlineCodeDefinitionCollection. Коллекция определений кода структуры, связанных с проектом. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Получает объект ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Получает все определения фильтров на основе ресурсов. ResourceFilters — это набор объектов[`Filter`](../filter). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Получает все определения групп на основе ресурсов. ResourceGroups — это набор объектов[`Group`](../group). |
| [Resources](../../aspose.tasks/project/resources) { get; } | Получает объект ResourceCollection. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Получает корень дерева задач. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Получает список объектов[`Table`](../table). |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Получает все определения фильтров на основе задач. TaskFilters — это набор объектов[`Filter`](../filter). |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Получает все определения групп на основе задач. TaskGroups — это набор объектов[`Group`](../group). |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Получает объект[`TaskLinkCollection`](../tasklinkcollection). |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Получает экземпляр класса[`VbaProject`](./vbaproject). |
| [Views](../../aspose.tasks/project/views) { get; } | Получает список объектов[`View`](../view). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Получает или задает определение кода WBS для проекта. |

## Методы

| Имя | Описание |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Копирует основные данные и свойства проекта в другой проект. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Копирует основные данные и свойства проекта в другой проект. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Рекурсивно перечисляет все задачи проекта, включая корневую задачу. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Возвращает значение, которому сопоставлено свойство в этом контейнере. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Возвращает базовое время сохранения. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Получает[`Duration`](../duration)объект с указанным количеством единиц и форматом продолжительности по умолчанию, который определен в настройках проекта[`DurationFormat`](../prj/durationformat). |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Получает[`Duration`](../duration)объект с указанным количеством[`TimeUnitType`](../timeunittype)единицы. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Получает[`Duration`](../duration)объект с указаннымTimeSpanзначением и указанное[`TimeUnitType`](../timeunittype)значение. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Возвращает количество страниц для проекта, который будет отображаться с использованием значения по умолчанию[`Timescale`](../../aspose.tasks.visualization/timescale)(дни). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Возвращает количество страниц для проекта, который будет отображаться с использованием значения по умолчанию[`Timescale`](../../aspose.tasks.visualization/timescale)(дней) и заданного[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`SaveOptions`](../../aspose.tasks.saving/saveoptions). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../aspose.tasks.visualization/timescale). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Возвращает количество страниц для проекта, который будет отображаться с использованием заданных[`Timescale`](../../aspose.tasks.visualization/timescale)и[`PageSize`](../../aspose.tasks.visualization/pagesize). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Возвращает количество страниц для проекта, который будет отображаться с использованием заданных[`Timescale`](../../aspose.tasks.visualization/timescale)и[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Возвращает количество страниц для проекта, который будет отображаться с использованием заданного[`Timescale`](../../aspose.tasks.visualization/timescale),[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat)и диапазон дат. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Возвращает набор ссылок на задачи, которые являются предшественниками указанной задачи. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Получает[`Duration`](../duration)объект с указаннымDoubleзначением и формат работы по умолчанию. |
| [Print](../../aspose.tasks/project/print#print)() | Печать проекта на принтер по умолчанию с настройками принтера по умолчанию с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Печать проекта в соответствии с заданными настройками принтера с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Печать проекта на принтер по умолчанию с настройками принтера по умолчанию и пользовательскими параметрами сохранения с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Распечатывает проект на указанный принтер с настройками принтера по умолчанию, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Печать проекта в соответствии с заданными настройками принтера и пользовательскими параметрами сохранения с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Печать проекта в соответствии с заданными настройками принтера с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Печать проекта в соответствии с указанными настройками принтера, пользовательскими параметрами сохранения и указанным именем документа с использованием стандартного (без пользовательского интерфейса) контроллера печати. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Перепланирует все идентификаторы задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и затрат. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Перепланирует все идентификаторы задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет резервы, поля работы и стоимости с дополнительной проверкой. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Пересчитывает идентификатор, начало и конец ресурсов. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Пересчитывает начало и конец ресурсов. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Удаляет недопустимые назначения ресурсов из списка назначений ресурсов проекта. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Перенумеровать СДР-код всех задач. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Перенумеровать СДР-код пройденных задач. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Перепланирует незавершенную проектную работу так, чтобы она началась после указанной даты. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Перепланирует незавершенную работу для указанного списка задач, чтобы начать после указанной даты. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Сохраняет данные проекта в файл в формате mpp. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Сохраняет проект в поток, используя указанные параметры сохранения. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Сохраняет данные проекта в поток. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Сохраняет проект в поток, используя указанные параметры сохранения. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Сохраняет документ в формате файла mpp, используя указанные параметры сохранения. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Сохраняет данные проекта в файл. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Сохраняет документ в файл, используя указанные параметры сохранения. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Сохраняет проект как шаблон в указанный поток. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Сохраняет проект как шаблон по указанному пути к файлу. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Сохраняет проект как шаблон в указанный поток. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Сохраняет проект как шаблон. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Сохраняет обзорный отчет проекта в поток. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Сохраняет обзорный отчет по проекту в файл PDF. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Сохраняет отчет по проекту указанного типа в указанный поток. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Сохраняет отчет по проекту указанного типа в формате PDF по указанному пути к файлу. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Рекурсивно собирает все дочерние задачи корневой задачи. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Сопоставляет указанное свойство с указанным значением в этом контейнере. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Сопоставляет указанное свойство с указанным значением в этом контейнере. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Сохраняет базовые поля в указанном базовом плане для всего проекта. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Сохраняет базовые поля в указанном базовом плане для выбранных задач. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Устанавливает базовое время сохранения. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Обновляет всю работу как завершенную до указанной даты для всего проекта. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Обновляет всю работу как завершенную до указанной даты для указанного списка задач. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Получает информацию о файле проекта из потока. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Читать информацию о файле проекта из файла. |

### Примечания

Проект это центральный класс в библиотеке Aspose.Tasks.

Можно использовать **Project** для чтения одного из поддерживаемых форматов управления проектами:MPP, MPT, MPX, XML.

Чтобы загрузить существующий документ в любом из поддерживаемых форматов, передайте имя файла или поток в один из проектов конструкторы. Чтобы создать пустой проект, вызовите конструктор без параметров.

Используйте одну из перегрузок метода Save для сохранения проекта в любом из форматов[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat):Primavera:P6 XML, PM XER; Microsoft Excel:XLSX, XML; Фиксированный макет:PDF; Изображения:JPEG, PNG, BMP, TIFF, SVG; Текст:ТХТ; Другое:HTML.

Чтобы распечатать проект, используйте одну из перегрузок метода[`Print`](./print).

Проект хранит информацию о проекте, такую как[`Views`](./views), [`BuiltInProps`](./builtinprops),[`CustomProps`](./customprops)и[`ExtendedAttributes`](./extendedattributes). Большинство этих объектов доступны через соответствующие свойства класса **Project** .

Проект — это корневой объект, который содержит точки входа для управления другими объектами проекта, такими как[`Task`](../task),[`Resource`](../resource),[`ResourceAssignment`](../resourceassignment),[`ExtendedAttribute`](../extendedattribute)и[`Calendar`](../calendar).

Проект объекты могут быть доступны через типизированные коллекции, например[`Children`](../task/children),[`Resources`](./resources),[`ResourceAssignments`](./resourceassignments), и т. д.

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
