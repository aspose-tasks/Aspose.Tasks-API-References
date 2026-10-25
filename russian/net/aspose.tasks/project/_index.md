---
title: "Класс Project"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Project. Представляет проект"
type: docs
weight: 1440
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
| [Project](project/#constructor)() | Инициализирует новый экземпляр класса `Project`. |
| [Project](project/#constructor_1)(DbSettings) | Инициализирует новый экземпляр класса `Project` для чтения данных из базы данных, указанной экземпляром класса [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/). |
| [Project](project/#constructor_2)(Stream) | Инициализирует новый экземпляр класса `Project` из потока. |
| [Project](project/#constructor_7)(StreamReader) | Инициализирует новый экземпляр класса `Project` из экземпляра StreamReader. |
| [Project](project/#constructor_8)(string) | Инициализирует новый экземпляр класса `Project` из шаблона (существующего файла mpp или mpt). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Инициализирует новый экземпляр класса `Project` из потока с указанным экземпляром класса [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Инициализирует новый экземпляр класса `Project` из шаблона(существующего файла mpp или mpt). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Инициализирует новый экземпляр класса `Project` из потока с указанным экземпляром класса [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_6)(Stream, string) | Инициализирует новый экземпляр класса `Project` из шаблона(существующего файла mpp или mpt). |
| [Project](project/#constructor_9)(string, LoadOptions) | Инициализирует новый экземпляр класса `Project` из шаблона (существующего файла mpp или mpt) с указанным экземпляром класса [`LoadOptions`](../loadoptions/). |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Инициализирует новый экземпляр класса `Project` из шаблона (существующего файла mpp или mpt). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Инициализирует новый экземпляр класса `Project` из шаблона (существующего файла MPP или MPT) с указанным экземпляром класса [`PrimaveraReadOptions`](../primaverareadoptions/). |
| [Project](project/#constructor_12)(string, string) | Инициализирует новый экземпляр класса `Project` из защищённого паролем шаблона (существующий файл mpp или mpt). |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Получает или задает значение, указывающее, установлен ли ActualsInSync, или нет. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Получает или задает значение, указывающее, установлен ли AdminProject, или нет. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Получает или задает значение, указывающее, установлен ли AreEditableActualCosts, или нет. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Получает или задает значение Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Получает или задает значение, указывающее, установлен ли AutoAddNewResourcesAndTasks, или нет. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Получает или задает, должны ли стоимость назначения и оставшаяся стоимость автоматически рассчитываться с использованием работы назначения и ставок ресурсов. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Получает или задает значение, указывающее, установлен ли Autolink, или нет. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Получает или задает значение BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Получает встроенную коллекцию свойств проекта. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Получает или задает режим расчёта проекта. Может быть одним из значений перечисления [`CalculationMode`](./calculationmode/). |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Получает или задает значение Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Получает объект [`CalendarCollection`](../calendarcollection/) данного экземпляра `Project`. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Получает или задает значение Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Получает или задает значение Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Получает или задает значение Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Получает или задает значение CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Получает коллекцию, содержащую список критических задач, составляющих критический путь этого проекта. Это операция O(n), где n — количество задач в проекте. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Задачи считаются критическими в MS Project, если общий резерв меньше или равен этому количеству дней. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Получает или задает значение CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Получает или задает значение CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Получает или задает значение CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Получает или задает значение CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Получает или задает значение CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Получает или задает значение CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Получает коллекцию пользовательских свойств проекта. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Получает или задает значение свойства DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Получает или задает значение свойства DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Получает или задает значение свойства DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Получает или задает значение свойства DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Получает или задает значение свойства DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Получает или задает значение свойства DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Получает или задает значение свойства DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Получает или задает значение свойства DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Получает или задает значение свойства DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Получает или задает представление проекта по умолчанию. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Получает экземпляр класса [`WeekDayCollection`](../weekdaycollection/), который представляет коллекцию стандартных рабочих дней недели проекта и их рабочее время. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Получает экземпляр класса [`ProjectDisplayOptions`](../projectdisplayoptions/). |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Получает или задает значение свойства DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Получает или задает значение свойства EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Получает объект ExtendedAttributeDefinitionCollection. Коллекция определений расширенных атрибутов (пользовательских полей), связанных с проектом. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Получает или задает значение свойства ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Получает или задает значение свойства FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Получает или задает значение, указывающее, установлен ли FiscalYearStart. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Получает или задает значение свойства FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Получает или задает глобализационные (языко-специфичные) настройки проекта. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Получает или задает значение Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Получает или задает значение, указывающее, установлен ли HonorConstraints. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Получает или задает значение свойства HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Получает или задает значение, указывающее, установлен ли InsertedProjectsLikeSummary. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Получает или задает значение, указывающее, установлен ли KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Получает или задает значение свойства Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Получает или задает значение LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Получает или задает значение LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Получает или задает значение LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Получает или задает значение Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Получает или задает значение, указывающее, установлен ли MicrosoftProjectServerURL. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Получает или задает значение MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Получает или задает значение MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Получает или задает значение, указывающее, установлен ли MoveCompletedEndsBack. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Получает или задает значение, указывающее, установлен ли MoveCompletedEndsForward. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Получает или задает значение, указывающее, установлен ли MoveRemainingStartsBack. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Получает или задает значение, указывающее, установлен ли MoveRemainingStartsForward. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Получает или задает значение, указывающее, установлен ли MultipleCriticalPaths. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Получает или задает значение свойства Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Получает или задает значение, указывающее, установлен ли NewTasksAreManual. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Получает или задает значение, указывающее, установлен ли NewTasksEffortDriven. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Получает или задает значение, указывающее, установлен ли NewTasksEstimated. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Получает или задает значение NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Получает коллекцию, содержащую экземпляры класса [`OleObject`](../oleobject/), связанные или встроенные в этот файл проекта. Доступно только для формата файла mpp. Эта коллекция доступна только для чтения, за исключением операции 'Clear'. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Получает объект OutlineCodeDefinitionCollection. Коллекция определений контурных кодов, связанных с проектом. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Получает объект, содержащий свойства, специфичные для Primavera, для проекта, считанного из файла Primavera. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Получает или задает значение, указывающее, установлен ли ProjectExternallyEdited. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Получает или задает значение, указывающее, установлен ли RemoveFileProperties. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Получает объект ResourceAssignmentCollection. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Получает все определения фильтров, основанных на ресурсах. ResourceFilters — это коллекция объектов [`Filter`](../filter/). |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Получает все определения групп, основанных на ресурсах. ResourceGroups — это коллекция объектов [`Group`](../group/). |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Получает объект ResourceCollection. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Получает или задает значение Revision. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Получает корень дерева задач. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Получает или задает значение SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Получает или задает значение, указывающее, установлен ли ScheduleFromStart. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Получает или задает значение, указывающее, установлен ли ShowProjectSummaryTask. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Получает или задает значение, указывающее, установлен ли SplitsInProgressTasks. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Получает или задает значение, указывающее, установлен ли SpreadActualCost. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Получает или задает значение, указывающее, установлен ли SpreadPercentComplete. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Получает или задает значение StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Получает или задает значение StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Получает или задает значение Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Получает список объектов [`Table`](../table/). |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Получает все определения фильтров, основанных на задачах. TaskFilters — это коллекция объектов [`Filter`](../filter/). |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Получает все определения групп, основанных на задачах. TaskGroups — это коллекция объектов [`Group`](../group/). |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Получает объект [`TaskLinkCollection`](../tasklinkcollection/). |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Получает или задает значение, указывающее, установлен ли TaskUpdatesResource. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Получает или задает значение Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Получает или задает значение TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Получает или задает значение TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Получает или задает значение Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Получает или задает значение Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Получает или задает значение, указывающее, установлен ли UpdateManuallyScheduledTasksWhenEditingLinks. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Получает экземпляр класса [`VbaProject`](./vbaproject/). |
| [Views](../../aspose.tasks/project/views/) { get; } | Получает список объектов [`View`](../view/). |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Получает или задает определение кода WBS для проекта. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Получает или задает значение WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Получает или задает значение WorkFormat. |

## Методы

| Имя | Описание |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Копирует основные данные и свойства проекта в другой проект. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Копирует основные данные и свойства проекта в другой проект. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Рекурсивно перечисляет все задачи проекта, включая корневую задачу. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Возвращает значение, к которому свойство сопоставлено в этом контейнере. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Возвращает время сохранения базовой линии. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Получает объект [`Duration`](../duration/) с указанным количеством единиц и форматом длительности по умолчанию, определённым в настройках проекта [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Получает объект [`Duration`](../duration/) с указанным количеством единиц [`TimeUnitType`](../timeunittype/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Получает объект [`Duration`](../duration/) с указанным значением TimeSpan и указанным значением [`TimeUnitType`](../timeunittype/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Возвращает количество страниц проекта, которое будет отрисовано с использованием масштаба времени по умолчанию [`Timescale`](../../aspose.tasks.visualization/timescale/)(Days). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Возвращает количество страниц проекта, которое будет отрисовано с использованием масштаба времени по умолчанию [`Timescale`](../../aspose.tasks.visualization/timescale/)(Days) и заданного формата представления [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Возвращает количество страниц проекта, которое будет отрисовано с использованием указанных параметров сохранения [`SaveOptions`](../../aspose.tasks.saving/saveoptions/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Возвращает количество страниц проекта, которое будет отрисовано с использованием указанного масштаба времени [`Timescale`](../../aspose.tasks.visualization/timescale/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Возвращает количество страниц проекта, которое будет отрисовано с использованием указанного масштаба времени [`Timescale`](../../aspose.tasks.visualization/timescale/) и размера страницы [`PageSize`](../../aspose.tasks.visualization/pagesize/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Возвращает количество страниц проекта, которое будет отрисовано с использованием указанного масштаба времени [`Timescale`](../../aspose.tasks.visualization/timescale/) и формата представления [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Возвращает количество страниц проекта, которое будет отрисовано с использованием указанного масштаба времени [`Timescale`](../../aspose.tasks.visualization/timescale/), формата представления [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) и диапазона дат. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Возвращает коллекцию связей задач, которые являются предшественниками указанной задачи. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Получает объект [`Duration`](../duration/) с указанным значением Double и форматом работы по умолчанию. |
| [Print](../../aspose.tasks/project/print/#print)() | Печатает проект на принтере по умолчанию с настройками принтера по умолчанию, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Печатает проект в соответствии с указанными настройками принтера, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Печатает проект на принтере по умолчанию с настройками принтера по умолчанию и пользовательскими параметрами сохранения, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Печатает проект на указанном принтере с настройками принтера по умолчанию, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Печатает проект в соответствии с указанными настройками принтера и пользовательскими параметрами сохранения, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Печатает проект в соответствии с указанными настройками принтера, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Печатает проект в соответствии с указанными настройками принтера, пользовательскими параметрами сохранения и указанным именем документа, используя стандартный (без пользовательского интерфейса) контроллер печати. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Перепланирует идентификаторы всех задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, работу и поля стоимости. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Перепланирует идентификаторы всех задач проекта, уровни структуры, даты начала/окончания, устанавливает ранние/поздние даты, вычисляет запасы времени, работу и поля стоимости с необязательной проверкой. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Пересчитывает идентификатор, дату начала и окончания ресурсов. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Удаляет недействительные назначения ресурсов из списка назначений ресурсов проекта. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Перенумеровывает код WBS всех задач. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Перенумеровывает код WBS прошедших задач. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Перепланирует незавершённую работу проекта, чтобы она начиналась после указанной даты. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Перепланирует незавершённую работу для указанного списка задач, чтобы она начиналась после указанной даты. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Сохраняет данные проекта в файл в формате mpp. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Сохраняет данные проекта в поток. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Сохраняет проект в поток, используя указанные параметры сохранения. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Сохраняет данные проекта в файл. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Сохраняет документ в файл, используя указанные параметры сохранения. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Сохраняет проект как шаблон в указанный поток. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Сохраняет проект как шаблон в указанный путь к файлу. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Сохраняет проект как шаблон в указанный поток. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Сохраняет проект как шаблон. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Сохраняет обзорный отчёт проекта в поток. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Сохраняет обзорный отчёт проекта в PDF‑файл. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Сохраняет отчёт проекта указанного типа в указанный поток. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Сохраняет отчёт проекта указанного типа в формате PDF в указанный путь к файлу. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Рекурсивно собирает все дочерние задачи корневой задачи. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Сопоставляет указанное свойство с указанным значением в этом контейнере. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Сопоставляет указанное свойство с указанным значением в этом контейнере. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Сохраняет поля базового плана в указанный базовый план для всего проекта. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Сохраняет поля базового плана в указанный базовый план для выбранных задач. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Устанавливает время сохранения базового плана. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Обновляет всю работу как завершённую до указанной даты для всего проекта. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Обновляет всю работу как завершённую до указанной даты для указанного списка задач. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Получает информацию о файле проекта из потока. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Читает информацию о файле проекта из файла. |

## Примечания

Класс **Project** является центральным классом в библиотеке Aspose.Tasks.

Можно использовать **Project** для чтения одного из поддерживаемых форматов управления проектами: MPP, MPT, MPX, XML.

Чтобы загрузить существующий документ в любом из поддерживаемых форматов, передайте имя файла или поток в один из конструкторов **Project**. Чтобы создать пустой проект, вызовите конструктор без параметров.

Используйте одну из перегрузок метода Save, чтобы сохранить проект в любом из форматов [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/): Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; фиксированная разметка: PDF; изображения: JPEG, PNG, BMP, TIFF, SVG; текст: TXT; другие: HTML.

**Project** хранит информацию уровня проекта, такую как [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), и [`ExtendedAttributes`](./extendedattributes/). Большинство этих объектов доступны через соответствующие свойства класса **Project**.

**Project** является корневой сущностью, содержащей точки входа для манипулирования другими сущностями проекта, такими как [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) и [`Calendar`](../calendar/).

Сущности **Project** могут быть доступны через типизированные коллекции, например [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), и т.д.

## Примеры

Показывает, как работать с экземпляром &lt;see cref="Aspose.Tasks.Project"/&gt;.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// добавление новых задач и установка желаемых свойств
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// добавление новых ресурсов
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// добавление новых назначений ресурсов
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// сохранить проект в одном из доступных форматов
// здесь мы сохраняем его в формате файла Microsoft Project XML.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


