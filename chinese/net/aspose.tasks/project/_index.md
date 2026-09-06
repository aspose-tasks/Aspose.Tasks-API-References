---
title: "类 Project"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Project 类。表示一个项目"
type: docs
weight: 1440
url: /zh/net/aspose.tasks/project/
---
## Project class

表示一个项目。

```csharp
public class Project
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [Project](project/#constructor)() | 初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_1)(DbSettings) | 初始化 `Project` 类的新实例，以从由[`DbSettings`](../../aspose.tasks.connectivity/dbsettings/)类实例指定的数据库读取数据。 |
| [Project](project/#constructor_2)(Stream) | 从流初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_7)(StreamReader) | 从 StreamReader 实例初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_8)(string) | 从模板（现有的 mpp 或 mpt 文件）初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_3)(Stream, LoadOptions) | 使用指定的[`LoadOptions`](../loadoptions/)类实例，从流初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | 从模板（现有的 mpp 或 mpt 文件）初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | 使用指定的[`PrimaveraReadOptions`](../primaverareadoptions/)类实例，从流初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_6)(Stream, string) | 从模板（现有的 mpp 或 mpt 文件）初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_9)(string, LoadOptions) | 从模板（现有的 mpp 或 mpt 文件）并使用指定的[`LoadOptions`](../loadoptions/)类实例初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | 从模板（现有的 mpp 或 mpt 文件）初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | 从模板（现有的 MPP 或 MPT 文件）并使用指定的[`PrimaveraReadOptions`](../primaverareadoptions/)类实例初始化 `Project` 类的新实例。 |
| [Project](project/#constructor_12)(string, string) | 从受密码保护的模板（现有的 mpp 或 mpt 文件）初始化 `Project` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | 获取或设置一个值，指示 ActualsInSync 是否已设置。 |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | 获取或设置一个值，指示 AdminProject 是否已设置。 |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | 获取或设置一个值，指示 AreEditableActualCosts 是否已设置。 |
| [Author](../../aspose.tasks/project/author/) { get; set; } | 获取或设置 Author 的值。 |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | 获取或设置一个值，指示 AutoAddNewResourcesAndTasks 是否已设置。 |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | 获取或设置是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | 获取或设置一个值，指示 Autolink 是否已设置。 |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | 获取或设置 BaselineForEarnedValue 的值。 |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | 获取项目的内置属性集合。 |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | 获取或设置项目的计算模式。可以是 [`CalculationMode`](./calculationmode/) 枚举的其中一个值。 |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | 获取或设置 Calendar 的值。 |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | 获取此 `Project` 实例的 [`CalendarCollection`](../calendarcollection/) 对象。 |
| [Category](../../aspose.tasks/project/category/) { get; set; } | 获取或设置 Category 的值。 |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | 获取或设置 Comments 的值。 |
| [Company](../../aspose.tasks/project/company/) { get; set; } | 获取或设置 Company 的值。 |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | 获取或设置 CreationDate 的值。 |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | 获取一个集合，其中包含构成此项目关键路径的关键任务列表。这是 O(n) 操作，其中 n 为项目中的任务数量。 |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | 如果总浮动小于或等于此天数，MS Project 将任务视为关键任务。 |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | 获取或设置 CurrencyCode 的值。 |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | 获取或设置 CurrencyDigits 的值。 |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | 获取或设置 CurrencySymbol 的值。 |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | 获取或设置 CurrencySymbolPosition 的值。 |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | 获取或设置 CurrentDate 的值。 |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | 获取或设置 CustomDateFormat 的值。 |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | 获取项目的自定义属性集合。 |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | 获取或设置 DateFormat 的值。 |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | 获取或设置 DaysPerMonth 的值。 |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | 获取或设置 DefaultFinishTime 的值。 |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | 获取或设置 DefaultFixedCostAccrual 的值。 |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | 获取或设置 DefaultOvertimeRate 的值。 |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | 获取或设置 DefaultStandardRate 的值。 |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | 获取或设置 DefaultStartTime 的值。 |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | 获取或设置 DefaultTaskEVMethod 的值。 |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | 获取或设置 DefaultTaskType 的值。 |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | 获取或设置项目的默认视图。 |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | 获取 [`WeekDayCollection`](../weekdaycollection/) 类的实例，该实例表示项目默认工作周的工作日和工作时间的集合。 |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | 获取 [`ProjectDisplayOptions`](../projectdisplayoptions/) 类的实例。 |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | 获取或设置 DurationFormat 的值。 |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | 获取或设置 EarnedValueMethod 的值。 |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | 获取 ExtendedAttributeDefinitionCollection 对象。该集合包含与项目关联的扩展属性（自定义字段）定义。 |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | 获取或设置 ExtendedCreationDate 的值。 |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | 获取或设置 FinishDate 的值。 |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | 获取或设置一个指示是否已设置 FiscalYearStart 的值。 |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | 获取或设置 FyStartDate 的值。 |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | 获取或设置项目的全球化（特定语言）设置。 |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | 获取或设置 Guid 的值。 |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | 获取或设置一个指示是否已设置 HonorConstraints 的值。 |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | 获取或设置 HyperlinkBase 的值。 |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | 获取或设置一个指示是否已设置 InsertedProjectsLikeSummary 的值。 |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | 获取或设置一个指示是否已设置 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 的值。 |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | 获取或设置 Keywords 的值。 |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | 获取或设置 LastAuthor 的值。 |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | 获取或设置 LastPrinted 的值。 |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | 获取或设置 LastSaved 的值。 |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | 获取或设置 Manager 的值。 |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | 获取或设置一个值，指示是否已设置 MicrosoftProjectServerURL。 |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | 获取或设置 MinutesPerDay 的值。 |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | 获取或设置 MinutesPerWeek 的值。 |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | 获取或设置一个值，指示是否已设置 MoveCompletedEndsBack。 |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | 获取或设置一个值，指示是否已设置 MoveCompletedEndsForward。 |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | 获取或设置一个值，指示是否已设置 MoveRemainingStartsBack。 |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | 获取或设置一个值，指示是否已设置 MoveRemainingStartsForward。 |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | 获取或设置一个值，指示是否已设置 MultipleCriticalPaths。 |
| [Name](../../aspose.tasks/project/name/) { get; set; } | 获取或设置 Name 的值。 |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | 获取或设置一个值，指示是否已设置 NewTasksAreManual。 |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | 获取或设置一个值，指示是否已设置 NewTasksEffortDriven。 |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | 获取或设置一个值，指示是否已设置 NewTasksEstimated。 |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | 获取或设置 NewTaskStartDate 的值。 |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | 获取一个集合，包含链接或嵌入到此项目文件的 [`OleObject`](../oleobject/) 类实例。仅适用于 mpp 文件格式。此集合是只读的，除 “Clear” 操作外。 |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | 获取 OutlineCodeDefinitionCollection 对象。该集合包含与项目关联的大纲代码定义。 |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | 获取一个对象，其中包含从 Primavera 文件读取的项目的 Primavera 特定属性。 |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | 获取或设置一个值，指示是否已设置 ProjectExternallyEdited。 |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | 获取或设置一个值，指示是否已设置 RemoveFileProperties。 |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | 获取 ResourceAssignmentCollection 对象。 |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | 获取所有基于资源的筛选器定义。ResourceFilters 是一个包含 [`Filter`](../filter/) 对象的集合。 |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | 获取所有基于资源的组定义。ResourceGroups 是一个包含 [`Group`](../group/) 对象的集合。 |
| [Resources](../../aspose.tasks/project/resources/) { get; } | 获取 ResourceCollection 对象。 |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | 获取或设置 Revision 的值。 |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | 获取任务树的根节点。 |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | 获取或设置 SaveVersion 的值。 |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | 获取或设置一个指示是否已设置 ScheduleFromStart 的值。 |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | 获取或设置一个指示是否已设置 ShowProjectSummaryTask 的值。 |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | 获取或设置一个指示是否已设置 SplitsInProgressTasks 的值。 |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | 获取或设置一个指示是否已设置 SpreadActualCost 的值。 |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | 获取或设置一个指示是否已设置 SpreadPercentComplete 的值。 |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | 获取或设置 StartDate 的值。 |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | 获取或设置 StatusDate 的值。 |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | 获取或设置 Subject 的值。 |
| [Tables](../../aspose.tasks/project/tables/) { get; } | 获取一个 [`Table`](../table/) 对象列表。 |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | 获取所有基于任务的过滤器定义。TaskFilters 是一个 [`Filter`](../filter/) 对象的集合。 |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | 获取所有基于任务的组定义。TaskGroups 是一个 [`Group`](../group/) 对象的集合。 |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | 获取 [`TaskLinkCollection`](../tasklinkcollection/) 对象。 |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | 获取或设置一个指示是否已设置 TaskUpdatesResource 的值。 |
| [Template](../../aspose.tasks/project/template/) { get; set; } | 获取或设置 Template 的值。 |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | 获取或设置 TimescaleFinish 的值。 |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | 获取或设置 TimescaleStart 的值。 |
| [Title](../../aspose.tasks/project/title/) { get; set; } | 获取或设置 Title 的值。 |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | 获取或设置 Uid 的值。 |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | 获取或设置一个指示是否已设置 UpdateManuallyScheduledTasksWhenEditingLinks 的值。 |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | 获取一个 [`VbaProject`](./vbaproject/) 类的实例。 |
| [Views](../../aspose.tasks/project/views/) { get; } | 获取一个 [`View`](../view/) 对象列表。 |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | 获取或设置项目的 WBS 代码定义。 |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | 获取或设置 WeekStartDay 的值。 |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | 获取或设置 WorkFormat 的值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | 将项目的主要数据和属性复制到另一个项目。 |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | 将项目的主要数据和属性复制到另一个项目。 |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | 递归枚举项目的所有任务，包括根任务。 |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | 返回属性在此容器中映射的值。 |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | 返回基准保存时间。 |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | 获取具有指定单位数和默认持续时间格式的 [`Duration`](../duration/) 对象，该默认持续时间格式在项目设置 [`DurationFormat`](../prj/durationformat/) 中定义。 |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | 获取具有指定数量的 [`TimeUnitType`](../timeunittype/) 单位的 [`Duration`](../duration/) 对象。 |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | 获取具有指定 TimeSpan 值和指定 [`TimeUnitType`](../timeunittype/) 值的 [`Duration`](../duration/) 对象。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | 返回使用默认 [`Timescale`](../../aspose.tasks.visualization/timescale/)（天）渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | 返回使用默认 [`Timescale`](../../aspose.tasks.visualization/timescale/)（天）和给定 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | 返回使用给定 [`SaveOptions`](../../aspose.tasks.saving/saveoptions/) 渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | 返回使用给定 [`Timescale`](../../aspose.tasks.visualization/timescale/) 渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | 返回使用给定 [`Timescale`](../../aspose.tasks.visualization/timescale/) 和 [`PageSize`](../../aspose.tasks.visualization/pagesize/) 渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | 返回使用给定 [`Timescale`](../../aspose.tasks.visualization/timescale/) 和 [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 渲染项目的页数。 |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | 返回使用给定 [`Timescale`](../../aspose.tasks.visualization/timescale/)、[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) 和日期范围渲染项目的页数。 |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | 返回指定任务的前置任务链接集合。 |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | 获取具有指定 Double 值和默认工作格式的 [`Duration`](../duration/) 对象。 |
| [Print](../../aspose.tasks/project/print/#print)() | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置。 |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置和自定义保存选项。 |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | 使用标准（无用户界面）打印控制器，将项目打印到指定打印机，使用默认打印机设置。 |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置和自定义保存选项打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置、自定义保存选项和指定的文档名称打印项目。 |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | 重新安排所有项目任务的 ID、大纲级别、开始/完成日期，设置提前/延后日期，计算浮动、工作和成本字段。 |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | 重新安排所有项目任务的 ID、大纲级别、开始/完成日期，设置提前/延后日期，计算浮动、工作和成本字段（可选验证）。 |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | 重新计算资源的 Id、开始和完成。 |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | 从项目资源分配列表中消除无效的资源分配。 |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | 重新编号所有任务的 WBS 代码。 |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | 重新编号已通过任务的 WBS 代码。 |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | 将未完成的项目工作重新安排在指定日期之后开始。 |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | 将指定任务列表的未完成工作重新安排在指定日期之后开始。 |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | 以 mpp 格式将项目数据保存到文件。 |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | 将项目数据保存到流中。 |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | 使用指定的保存选项将项目保存到流中。 |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | 将项目数据保存到文件。 |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | 使用指定的保存选项将文档保存到文件。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | 将项目作为模板保存到指定的流中。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | 将项目作为模板保存到指定的文件路径。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | 将项目作为模板保存到指定的流中。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | 将项目保存为模板。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | 将项目概览报告保存到流中。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | 将项目概览报告保存为 PDF 文件。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | 将指定类型的项目报告保存到指定的流中。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | 将指定类型的项目报告以 PDF 格式保存到指定的文件路径。 |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | 递归收集根任务的所有子任务。 |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | 将指定属性映射到此容器中的指定值。 |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | 将指定属性映射到此容器中的指定值。 |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | 将基线字段保存到整个项目的指定基线。 |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | 将基线字段保存到所选任务的指定基线。 |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | 设置基线保存时间。 |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | 将整个项目的所有工作更新为在指定日期之前完成。 |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | 将指定任务列表的所有工作更新为在指定日期之前完成。 |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | 从流中获取项目文件信息。 |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | 从文件读取项目文件信息。 |

## 备注

该 **Project** 是 Aspose.Tasks 库中的核心类。

可以使用 **Project** 读取受支持的项目管理格式之一：MPP、MPT、MPX、XML。

要在任何受支持的格式中加载现有文档，需将文件名或流传入 **Project** 的其中一个构造函数。要创建空项目，请调用无参数构造函数。

使用 Save 方法的其中一个重载将项目保存为以下任意 [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) 格式：Primavera：P6 XML、PM XER；Microsoft Excel：XLSX、XML；固定布局：PDF；图像：JPEG、PNG、BMP、TIFF、SVG；文本：TXT；其他：HTML。

**Project** 存储项目范围的信息，例如 [`Views`](./views/)、[`BuiltInProps`](./builtinprops/)、[`CustomProps`](./customprops/) 和 [`ExtendedAttributes`](./extendedattributes/)。这些对象的大多数可通过 **Project** 类的相应属性访问。

**Project** 是根实体，包含用于操作其他项目实体的入口点，例如 [`Task`](../task/)、[`Resource`](../resource/)、[`ResourceAssignment`](../resourceassignment/)、[`ExtendedAttribute`](../extendedattribute/) 和 [`Calendar`](../calendar/)。

**Project** 实体可以通过类型化集合访问，例如 [`Children`](../task/children/)、[`Resources`](./resources/)、[`ResourceAssignments`](./resourceassignments/) 等。

## 示例

Shows how to work with a &lt;see cref=\"Aspose.Tasks.Project\"/&gt; 实例。

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// 添加新任务并设置所需属性
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// 添加新资源
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// 添加新资源分配
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// 将项目保存为可用格式之一
// 这里我们将其保存为 Microsoft Project XML 文件格式。
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


