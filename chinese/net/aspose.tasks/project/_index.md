---
title: Class Project
second_title: Aspose.Tasks for .NET API 参考
description: Aspose.Tasks.Project 班级. 代表一个项目
type: docs
weight: 1190
url: /zh/net/aspose.tasks/project/
---
## Project class

代表一个项目。

```csharp
public class Project
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Project](project/#constructor)() | 初始化一个新的实例`Project`类. |
| [Project](project/#constructor_1)(DbSettings) | 初始化一个新的实例`Project`类从实例指定的数据库中读取数据[`DbSettings`](../../aspose.tasks.connectivity/dbsettings/)类. |
| [Project](project/#constructor_2)(Stream) | 初始化一个新的实例`Project`来自流的类. |
| [Project](project/#constructor_7)(StreamReader) | 初始化一个新的实例`Project`来自 StreamReader 实例的类。 |
| [Project](project/#constructor_8)(string) | 初始化一个新的实例`Project`来自模板的类（现有的 mpp 或 mpt 文件）. |
| [Project](project/#constructor_3)(Stream, LoadOptions) | 初始化一个新的实例`Project`来自具有指定实例的 Stream 的类[`LoadOptions`](../loadoptions/)类. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | 初始化一个新的实例`Project`来自模板的类（现有的 mpp 或 mpt 文件）. |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | 初始化一个新的实例`Project`来自具有指定实例的 Stream 的类[`PrimaveraReadOptions`](../primaverareadoptions/)类. |
| [Project](project/#constructor_6)(Stream, string) | 初始化一个新的实例`Project`来自模板的类（现有的 mpp 或 mpt 文件）. |
| [Project](project/#constructor_9)(string, LoadOptions) | 初始化一个新的实例`Project`来自模板的类（现有的 mpp 或 mpt 文件） 具有指定的实例[`LoadOptions`](../loadoptions/)类. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | 初始化一个新的实例`Project`来自模板的类（现有的 mpp 或 mpt 文件）. |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | 初始化一个新的实例`Project`来自模板（现有 MPP 或 MPT 文件） 的类，具有[`PrimaveraReadOptions`](../primaverareadoptions/)类. |
| [Project](project/#constructor_12)(string, string) | 初始化一个新的实例`Project`来自受密码保护的模板（现有的 mpp 或 mpt 文件）的类。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | 获取或设置一个值，该值指示是否设置了 ActualsInSync。 |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | 获取或设置一个值，指示 AdminProject 是否已设置。 |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | 获取或设置一个值，该值指示是否设置了 AreEditableActualCosts。 |
| [Author](../../aspose.tasks/project/author/) { get; set; } | 获取或设置 Author. 的值 |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | 获取或设置一个值，指示是否设置了 AutoAddNewResourcesAndTasks。 |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | 获取或设置一个值，指示是否设置了自动链接。 |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | 获取或设置 BaselineForEarnedValue 的值。 |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | 获取项目的内置属性集合。 |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | 获取或设置项目的计算模式。 可以是以下值之一[`CalculationMode`](./calculationmode/)枚举. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | 获取或设置日历的值。 |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | 获取[`CalendarCollection`](../calendarcollection/)此项目实例的对象. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | 获取或设置类别的值。 |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | 获取或设置 Comments 的值。 |
| [Company](../../aspose.tasks/project/company/) { get; set; } | 获取或设置公司的值。 |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | 获取或设置 CreationDate 的值。 |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | 获取一个集合，其中包含构成该项目关键路径的关键任务列表。 这是一个 O(n) 操作，其中 n 是项目中的任务数。 |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | 获取或设置 CriticalSlackLimit 的值。 |
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
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | 获取实例[`WeekDayCollection`](../weekdaycollection/)表示项目默认周工作日和工作时间集合的类。 |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | 获取一个实例[`ProjectDisplayOptions`](../projectdisplayoptions/)类. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | 获取或设置 DurationFormat 的值。 |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | 获取或设置 EarnedValueMethod 的值。 |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | 获取 ExtendedAttributeDefinitionCollection 对象。 与项目关联的扩展属性（自定义字段）定义的集合。 |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | 获取或设置 ExtendedCreationDate 的值。 |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | 获取或设置 FinishDate 的值。 |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | 获取或设置一个值，该值指示 FiscalYearStart 是否已设置。 |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | 获取或设置 FyStartDate 的值。 |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | 获取或设置 Guid 的值。 |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | 获取或设置是否设置 HonorConstraints 的值。 |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | 获取或设置 HyperlinkBase 的值。 |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | 获取或设置一个值，指示 InsertedProjectsLikeSummary 是否已设置。 |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | 获取或设置一个值，该值指示是否设置了 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled。 |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | 获取或设置关键字的值。 |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | 获取或设置 LastAuthor 的值。 |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | 获取或设置 LastPrinted 的值。 |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | 获取或设置 LastSaved 的值。 |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | 获取或设置 Manager 的值。 |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | 获取或设置一个值，指示是否设置了 MicrosoftProjectServerURL。 |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | 获取或设置 MinutesPerDay 的值。 |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | 获取或设置 MinutesPerWeek 的值。 |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | 获取或设置一个值，指示是否设置了 MoveCompletedEndsBack。 |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | 获取或设置一个值，指示是否设置了 MoveCompletedEndsForward。 |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | 获取或设置一个值，指示是否设置了 MoveRemainingStartsBack。 |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | 获取或设置一个值，指示是否设置了 MoveRemainingStartsForward。 |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | 获取或设置一个值，该值指示是否设置了 MultipleCriticalPaths。 |
| [Name](../../aspose.tasks/project/name/) { get; set; } | 获取或设置 Name. 的值 |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | 获取或设置一个值，指示是否设置了 NewTasksAreManual。 |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | 获取或设置一个值，该值指示是否设置了 NewTasksEffortDriven。 |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | 获取或设置一个值，该值指示是否设置了 NewTasksEstimated。 |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | 获取或设置 NewTaskStartDate 的值。 |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | 获取包含的实例的集合[`OleObject`](../oleobject/)链接或嵌入到此项目文件的类。 仅适用于 mpp 文件格式。除了“清除”操作外，此集合是只读的。 |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | 获取 OutlineCodeDefinitionCollection 对象。 与项目关联的大纲代码定义的集合。 |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | 获取或设置一个值，该值指示是否设置了 ProjectExternallyEdited。 |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | 获取或设置一个值，该值指示是否设置了 RemoveFileProperties。 |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | 获取 ResourceAssignmentCollection 对象。 |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | 获取所有基于资源的过滤器定义。 ResourceFilters 是一个集合[`Filter`](../filter/)对象. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | 获取所有基于资源的组定义。 ResourceGroups 是一个集合[`Group`](../group/)对象. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | 获取 ResourceCollection 对象。 |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | 获取或设置 Revision 的值。 |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | 获取任务树的根。 |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | 获取或设置 SaveVersion 的值。 |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | 获取或设置一个值，该值指示是否设置了 ScheduleFromStart。 |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | 获取或设置一个值，指示是否设置了 ShowProjectSummaryTask。 |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | 获取或设置一个值，该值指示是否设置了 SplitsInProgressTasks。 |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | 获取或设置一个值，该值指示是否设置了 SpreadActualCost。 |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | 获取或设置一个值，该值指示是否设置了 SpreadPercentComplete。 |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | 获取或设置 StartDate 的值。 |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | 获取或设置 StatusDate 的值。 |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | 获取或设置 Subject 的值。 |
| [Tables](../../aspose.tasks/project/tables/) { get; } | 获取列表[`Table`](../table/)对象. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | 获取所有基于任务的过滤器定义。 TaskFilters 是一个集合[`Filter`](../filter/)对象. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | 获取所有基于任务的组定义。 TaskGroups 是一个集合[`Group`](../group/)对象. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | 获取[`TaskLinkCollection`](../tasklinkcollection/)对象. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | 获取或设置一个值，指示是否设置了 TaskUpdatesResource。 |
| [Template](../../aspose.tasks/project/template/) { get; set; } | 获取或设置模板的值。 |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | 获取或设置 TimescaleFinish 的值。 |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | 获取或设置 TimescaleStart 的值。 |
| [Title](../../aspose.tasks/project/title/) { get; set; } | 获取或设置 Title 的值。 |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | 获取或设置 Uid 的值。 |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | 获取或设置一个值，该值指示是否设置了 UpdateManuallyScheduledTasksWhenEditingLinks。 |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | 获取一个实例[`VbaProject`](./vbaproject/)类. |
| [Views](../../aspose.tasks/project/views/) { get; } | 获取列表[`View`](../view/)对象. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | 获取或设置项目的 WBS 代码定义。 |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | 获取或设置 WeekStartDay 的值。 |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | 获取或设置 WorkFormat 的值。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | 将项目的主要数据和属性复制到另一个项目。 |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | 将项目的主要数据和属性复制到另一个项目。 |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | 递归枚举所有项目的任务，包括根任务。 |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | 返回此容器中属性映射到的值。 |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | 返回基线保存时间。 |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | 获取[`Duration`](../duration/)具有在项目设置中定义的指定单位数和默认持续时间格式的对象[`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | 获取[`Duration`](../duration/)具有指定数量的对象[`TimeUnitType`](../timeunittype/)单位. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | 获取[`Duration`](../duration/)具有指定对象TimeSpan值和指定[`TimeUnitType`](../timeunittype/)值. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | 返回要使用默认呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/)（天）. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | 返回要使用默认呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/) （天）并给予[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | 返回要使用给定呈现的项目的页数[`SaveOptions`](../../aspose.tasks.saving/saveoptions/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | 返回要使用给定呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | 返回要使用给定呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/)和[`PageSize`](../../aspose.tasks.visualization/pagesize/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | 返回要使用给定呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/)和[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | 返回要使用给定呈现的项目的页数[`Timescale`](../../aspose.tasks.visualization/timescale/),[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/)和日期范围. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | 返回任务链接的集合，这些链接是指定任务的前置任务。 |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | 获取[`Duration`](../duration/)具有指定对象Double值和默认工作格式. |
| [Print](../../aspose.tasks/project/print/#print)() | 使用标准（无用户界面）打印控制器使用默认打印机设置将项目打印到默认打印机。 |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | 使用标准（无用户界面）打印控制器根据指定的打印机设置打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | 使用标准（无用户界面）打印控制器使用默认打印机设置和自定义保存选项将项目打印到默认打印机。 |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | 使用标准（无用户界面）打印控制器使用默认打印机设置将项目打印到指定打印机。 |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | 使用标准（无用户界面）打印控制器根据指定的打印机设置和自定义保存选项打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | 使用标准（无用户界面）打印控制器根据指定的打印机设置打印项目。 |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | 使用标准（无用户界面）打印控制器根据指定的打印机设置、自定义保存选项和指定的文档名称打印项目。 |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | 重新安排所有项目任务 ID、大纲级别、开始/结束日期、设置早/晚日期、计算松弛时间、工时和成本字段。 |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | 重新安排所有项目任务 ID、大纲级别、开始/结束日期、设置早/晚日期、计算松弛时间、工作和成本字段以及可选验证。 |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | 重新计算资源的 ID、开始和结束。 |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish/)() | 重新计算资源的开始和结束。 |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | 从项目资源分配列表中删除无效的资源分配。 |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | 重新编号所有任务的 WBS 代码。 |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | 重新编号已通过任务的 WBS 代码。 |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | 重新安排未完成的项目工作在指定日期后开始。 |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | 重新安排指定任务列表中未完成的工作在指定日期后开始。 |
| [Save](../../aspose.tasks/project/save/#save_3)(string) | 将项目数据以mpp格式保存到文件中。 |
| [Save](../../aspose.tasks/project/save/#save)(Stream, MPPSaveOptions) | 使用指定的保存选项将项目保存到流中。 |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SaveFileFormat) | 将项目数据保存到流中。 |
| [Save](../../aspose.tasks/project/save/#save_2)(Stream, SaveOptions) | 使用指定的保存选项将项目保存到流中。 |
| [Save](../../aspose.tasks/project/save/#save_4)(string, MPPSaveOptions) | 使用指定的保存选项将文档保存为 mpp 文件格式。 |
| [Save](../../aspose.tasks/project/save/#save_5)(string, SaveFileFormat) | 将项目数据保存到文件中。 |
| [Save](../../aspose.tasks/project/save/#save_6)(string, SaveOptions) | 使用指定的保存选项将文档保存到文件。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | 将项目作为模板保存到指定流。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | 将项目作为模板保存到指定的文件路径。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | 将项目作为模板保存到指定流。 |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | 将项目另存为模板。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | 将项目概览报告保存到流中。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | 将项目概览报告保存为 PDF 文件。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | 将指定类型的工程报表保存到指定流中。 |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | 将指定类型的工程报表以PDF格式保存到指定文件路径下。 |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | 递归收集根任务的所有子任务。 |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | 将指定属性映射到此容器中的指定值。 |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | 将指定属性映射到此容器中的指定值。 |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | 将基线字段保存到整个项目的指定基线。 |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | 将基线字段保存到所选任务的指定基线。 |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | 设置基线保存时间。 |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | 将整个项目的指定日期内的所有工作更新为已完成。 |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | 将指定任务列表的指定日期的所有工作更新为已完成。 |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | 从流中获取项目文件信息。 |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | 从文件中读取项目文件信息。 |

### 评论

这 **项目**是 Aspose.Tasks 库中的核心类。

可以使用 **项目**阅读其中一种受支持的项目管理格式：MPP、MPT、MPX、XML.

要以任何支持的格式加载现有文档，请将文件名或流传递到其中一个 **项目**构造函数。要创建一个空白项目，请调用无参数构造函数。

使用 Save 方法重载之一将项目保存在任何[`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/)格式：Primavera：P6 XML、PM XER；微软 Excel：XLSX、XML；固定布局：PDF；图片：JPEG、PNG、BMP、TIFF、SVG；文字：TXT；其他：HTML。

要打印项目，请使用其中一种[`Print`](./print/)方法重载。

这 **项目**存储项目范围的信息，例如[`Views`](./views/)[`BuiltInProps`](./builtinprops/),[`CustomProps`](./customprops/) ， 和[`ExtendedAttributes`](./extendedattributes/). 大多数这些对象都可以通过相应的属性访问 **项目**班级。

这 **项目**是一个根实体，包含用于操作其他项目实体的入口点，例如[`Task`](../task/),[`Resource`](../resource/),[`ResourceAssignment`](../resourceassignment/),[`ExtendedAttribute`](../extendedattribute/)和[`Calendar`](../calendar/).

的 **项目**可以通过类型化集合访问实体，例如[`Children`](../task/children/),[`Resources`](./resources/),[`ResourceAssignments`](./resourceassignments/)等

### 也可以看看

* 命名空间 [Aspose.Tasks](../../aspose.tasks/)
* 部件 [Aspose.Tasks](../../)


