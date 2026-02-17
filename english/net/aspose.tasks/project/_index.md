---
title: Class Project
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Project class. Represents a project
type: docs
weight: 1420
url: /net/aspose.tasks/project/
---
## Project class

Represents a project.

```csharp
public class Project
```

## Constructors

| Name | Description |
| --- | --- |
| [Project](project/#constructor)() | Initializes a new instance of the `Project` class. |
| [Project](project/#constructor_1)(DbSettings) | Initializes a new instance of the `Project` class to read data from a database which is specified by the instance of the [`DbSettings`](../../aspose.tasks.connectivity/dbsettings/) class. |
| [Project](project/#constructor_2)(Stream) | Initializes a new instance of the `Project` class from a stream. |
| [Project](project/#constructor_7)(StreamReader) | Initializes a new instance of the `Project` class from a StreamReader instance. |
| [Project](project/#constructor_8)(string) | Initializes a new instance of the `Project` class from a template (existent mpp or mpt file). |
| [Project](project/#constructor_3)(Stream, LoadOptions) | Initializes a new instance of the `Project` class from the Stream with the specified instance of the [`LoadOptions`](../loadoptions/) class. |
| [Project](project/#constructor_4)(Stream, ParseErrorCallback) | Initializes a new instance of the `Project` class from a template(existent mpp or mpt file). |
| [Project](project/#constructor_5)(Stream, PrimaveraReadOptions) | Initializes a new instance of the `Project` class from the Stream with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions/) class. |
| [Project](project/#constructor_6)(Stream, string) | Initializes a new instance of the `Project` class from a template(existent mpp or mpt file). |
| [Project](project/#constructor_9)(string, LoadOptions) | Initializes a new instance of the `Project` class from a template (existent mpp or mpt file) with the specified instance of the [`LoadOptions`](../loadoptions/) class. |
| [Project](project/#constructor_10)(string, ParseErrorCallback) | Initializes a new instance of the `Project` class from a template (existent mpp or mpt file). |
| [Project](project/#constructor_11)(string, PrimaveraReadOptions) | Initializes a new instance of the `Project` class from a template (existent MPP or MPT file) with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions/) class. |
| [Project](project/#constructor_12)(string, string) | Initializes a new instance of the `Project` class from a password protected template (existent mpp or mpt file). |

## Properties

| Name | Description |
| --- | --- |
| [ActualsInSync](../../aspose.tasks/project/actualsinsync/) { get; set; } | Gets or sets a value indicating whether ActualsInSync is set or not. |
| [AdminProject](../../aspose.tasks/project/adminproject/) { get; set; } | Gets or sets a value indicating whether AdminProject is set or not. |
| [AreEditableActualCosts](../../aspose.tasks/project/areeditableactualcosts/) { get; set; } | Gets or sets a value indicating whether AreEditableActualCosts is set or not. |
| [Author](../../aspose.tasks/project/author/) { get; set; } | Gets or sets a value of Author. |
| [AutoAddNewResourcesAndTasks](../../aspose.tasks/project/autoaddnewresourcesandtasks/) { get; set; } | Gets or sets a value indicating whether AutoAddNewResourcesAndTasks is set or not. |
| [AutoCalculateAssignmentCosts](../../aspose.tasks/project/autocalculateassignmentcosts/) { get; set; } | Gets or sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |
| [Autolink](../../aspose.tasks/project/autolink/) { get; set; } | Gets or sets a value indicating whether Autolink is set or not. |
| [BaselineForEarnedValue](../../aspose.tasks/project/baselineforearnedvalue/) { get; set; } | Gets or sets a value of BaselineForEarnedValue. |
| [BuiltInProps](../../aspose.tasks/project/builtinprops/) { get; } | Gets project's built-in properties collection. |
| [CalculationMode](../../aspose.tasks/project/calculationmode/) { get; set; } | Gets or sets calculation mode of a project. Can be one of the values of [`CalculationMode`](./calculationmode/) enumeration. |
| [Calendar](../../aspose.tasks/project/calendar/) { get; set; } | Gets or sets a value of Calendar. |
| [Calendars](../../aspose.tasks/project/calendars/) { get; } | Gets [`CalendarCollection`](../calendarcollection/) object of this Project instance. |
| [Category](../../aspose.tasks/project/category/) { get; set; } | Gets or sets a value of Category. |
| [Comments](../../aspose.tasks/project/comments/) { get; set; } | Gets or sets a value of Comments. |
| [Company](../../aspose.tasks/project/company/) { get; set; } | Gets or sets a value of Company. |
| [CreationDate](../../aspose.tasks/project/creationdate/) { get; set; } | Gets or sets a value of CreationDate. |
| [CriticalPath](../../aspose.tasks/project/criticalpath/) { get; } | Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. This is an O(n) operation, where n is the number of tasks in the project. |
| [CriticalSlackLimit](../../aspose.tasks/project/criticalslacklimit/) { get; set; } | Tasks are considered critical by MS Project if total slack is less or equal to this number of days. |
| [CurrencyCode](../../aspose.tasks/project/currencycode/) { get; set; } | Gets or sets a value of CurrencyCode. |
| [CurrencyDigits](../../aspose.tasks/project/currencydigits/) { get; set; } | Gets or sets a value of CurrencyDigits. |
| [CurrencySymbol](../../aspose.tasks/project/currencysymbol/) { get; set; } | Gets or sets a value of CurrencySymbol. |
| [CurrencySymbolPosition](../../aspose.tasks/project/currencysymbolposition/) { get; set; } | Gets or sets a value of CurrencySymbolPosition. |
| [CurrentDate](../../aspose.tasks/project/currentdate/) { get; set; } | Gets or sets a value of CurrentDate. |
| [CustomDateFormat](../../aspose.tasks/project/customdateformat/) { get; set; } | Gets or sets a value of CustomDateFormat. |
| [CustomProps](../../aspose.tasks/project/customprops/) { get; } | Gets project's custom properties collection. |
| [DateFormat](../../aspose.tasks/project/dateformat/) { get; set; } | Gets or sets a value of DateFormat. |
| [DaysPerMonth](../../aspose.tasks/project/dayspermonth/) { get; set; } | Gets or sets a value of DaysPerMonth. |
| [DefaultFinishTime](../../aspose.tasks/project/defaultfinishtime/) { get; set; } | Gets or sets a value of DefaultFinishTime. |
| [DefaultFixedCostAccrual](../../aspose.tasks/project/defaultfixedcostaccrual/) { get; set; } | Gets or sets a value of DefaultFixedCostAccrual. |
| [DefaultOvertimeRate](../../aspose.tasks/project/defaultovertimerate/) { get; set; } | Gets or sets a value of DefaultOvertimeRate. |
| [DefaultStandardRate](../../aspose.tasks/project/defaultstandardrate/) { get; set; } | Gets or sets a value of DefaultStandardRate. |
| [DefaultStartTime](../../aspose.tasks/project/defaultstarttime/) { get; set; } | Gets or sets a value of DefaultStartTime. |
| [DefaultTaskEVMethod](../../aspose.tasks/project/defaulttaskevmethod/) { get; set; } | Gets or sets a value of DefaultTaskEVMethod. |
| [DefaultTaskType](../../aspose.tasks/project/defaulttasktype/) { get; set; } | Gets or sets a value of DefaultTaskType. |
| [DefaultView](../../aspose.tasks/project/defaultview/) { get; set; } | Gets or sets default view of the project. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays/) { get; } | Gets the instance of [`WeekDayCollection`](../weekdaycollection/) class which represents a collection of project default week working days and working times. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions/) { get; } | Gets an instance of the [`ProjectDisplayOptions`](../projectdisplayoptions/) class. |
| [DurationFormat](../../aspose.tasks/project/durationformat/) { get; set; } | Gets or sets a value of DurationFormat. |
| [EarnedValueMethod](../../aspose.tasks/project/earnedvaluemethod/) { get; set; } | Gets or sets a value of EarnedValueMethod. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes/) { get; } | Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project. |
| [ExtendedCreationDate](../../aspose.tasks/project/extendedcreationdate/) { get; set; } | Gets or sets a value of ExtendedCreationDate. |
| [FinishDate](../../aspose.tasks/project/finishdate/) { get; set; } | Gets or sets a value of FinishDate. |
| [FiscalYearStart](../../aspose.tasks/project/fiscalyearstart/) { get; set; } | Gets or sets a value indicating whether FiscalYearStart is set or not. |
| [FyStartDate](../../aspose.tasks/project/fystartdate/) { get; set; } | Gets or sets a value of FyStartDate. |
| [GlobalizationSettings](../../aspose.tasks/project/globalizationsettings/) { get; set; } | Gets or sets globalization (language-specific) settings of the project. |
| [Guid](../../aspose.tasks/project/guid/) { get; set; } | Gets or sets a value of Guid. |
| [HonorConstraints](../../aspose.tasks/project/honorconstraints/) { get; set; } | Gets or sets a value indicating whether HonorConstraints is set or not. |
| [HyperlinkBase](../../aspose.tasks/project/hyperlinkbase/) { get; set; } | Gets or sets a value of HyperlinkBase. |
| [InsertedProjectsLikeSummary](../../aspose.tasks/project/insertedprojectslikesummary/) { get; set; } | Gets or sets a value indicating whether InsertedProjectsLikeSummary is set or not. |
| [KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](../../aspose.tasks/project/keeptaskonnearestworkingtimewhenmadeautoscheduled/) { get; set; } | Gets or sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |
| [Keywords](../../aspose.tasks/project/keywords/) { get; set; } | Gets or sets a value of Keywords. |
| [LastAuthor](../../aspose.tasks/project/lastauthor/) { get; set; } | Gets or sets a value of LastAuthor. |
| [LastPrinted](../../aspose.tasks/project/lastprinted/) { get; set; } | Gets or sets a value of LastPrinted. |
| [LastSaved](../../aspose.tasks/project/lastsaved/) { get; set; } | Gets or sets a value of LastSaved. |
| [Manager](../../aspose.tasks/project/manager/) { get; set; } | Gets or sets a value of Manager. |
| [MicrosoftProjectServerURL](../../aspose.tasks/project/microsoftprojectserverurl/) { get; set; } | Gets or sets a value indicating whether MicrosoftProjectServerURL is set or not. |
| [MinutesPerDay](../../aspose.tasks/project/minutesperday/) { get; set; } | Gets or sets a value of MinutesPerDay. |
| [MinutesPerWeek](../../aspose.tasks/project/minutesperweek/) { get; set; } | Gets or sets a value of MinutesPerWeek. |
| [MoveCompletedEndsBack](../../aspose.tasks/project/movecompletedendsback/) { get; set; } | Gets or sets a value indicating whether MoveCompletedEndsBack is set or not. |
| [MoveCompletedEndsForward](../../aspose.tasks/project/movecompletedendsforward/) { get; set; } | Gets or sets a value indicating whether MoveCompletedEndsForward is set or not. |
| [MoveRemainingStartsBack](../../aspose.tasks/project/moveremainingstartsback/) { get; set; } | Gets or sets a value indicating whether MoveRemainingStartsBack is set or not. |
| [MoveRemainingStartsForward](../../aspose.tasks/project/moveremainingstartsforward/) { get; set; } | Gets or sets a value indicating whether MoveRemainingStartsForward is set or not. |
| [MultipleCriticalPaths](../../aspose.tasks/project/multiplecriticalpaths/) { get; set; } | Gets or sets a value indicating whether MultipleCriticalPaths is set or not. |
| [Name](../../aspose.tasks/project/name/) { get; set; } | Gets or sets a value of Name. |
| [NewTasksAreManual](../../aspose.tasks/project/newtasksaremanual/) { get; set; } | Gets or sets a value indicating whether NewTasksAreManual is set or not. |
| [NewTasksEffortDriven](../../aspose.tasks/project/newtaskseffortdriven/) { get; set; } | Gets or sets a value indicating whether NewTasksEffortDriven is set or not. |
| [NewTasksEstimated](../../aspose.tasks/project/newtasksestimated/) { get; set; } | Gets or sets a value indicating whether NewTasksEstimated is set or not. |
| [NewTaskStartDate](../../aspose.tasks/project/newtaskstartdate/) { get; set; } | Gets or sets a value of NewTaskStartDate. |
| [OleObjects](../../aspose.tasks/project/oleobjects/) { get; } | Gets a collection containing the instances of the [`OleObject`](../oleobject/) class which are linked or embedded to this project file. Available for mpp file format only. This collection is read-only except for 'Clear' operation. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes/) { get; } | Gets OutlineCodeDefinitionCollection object. The collection of outline code definitions associated with a project. |
| [PrimaveraProperties](../../aspose.tasks/project/primaveraproperties/) { get; } | Gets an object containing Primavera-specific properties for a project read from Primavera file. |
| [ProjectExternallyEdited](../../aspose.tasks/project/projectexternallyedited/) { get; set; } | Gets or sets a value indicating whether ProjectExternallyEdited is set or not. |
| [RemoveFileProperties](../../aspose.tasks/project/removefileproperties/) { get; set; } | Gets or sets a value indicating whether RemoveFileProperties is set or not. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments/) { get; } | Gets ResourceAssignmentCollection object. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters/) { get; } | Gets all the resource-based filter definitions. ResourceFilters is a collection of [`Filter`](../filter/) objects. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups/) { get; } | Gets all of the resource-based group definitions. ResourceGroups is a collection of [`Group`](../group/) objects. |
| [Resources](../../aspose.tasks/project/resources/) { get; } | Gets ResourceCollection object. |
| [Revision](../../aspose.tasks/project/revision/) { get; set; } | Gets or sets a value of Revision. |
| [RootTask](../../aspose.tasks/project/roottask/) { get; } | Gets the root of the tree of tasks. |
| [SaveVersion](../../aspose.tasks/project/saveversion/) { get; set; } | Gets or sets a value of SaveVersion. |
| [ScheduleFromStart](../../aspose.tasks/project/schedulefromstart/) { get; set; } | Gets or sets a value indicating whether ScheduleFromStart is set or not. |
| [ShowProjectSummaryTask](../../aspose.tasks/project/showprojectsummarytask/) { get; set; } | Gets or sets a value indicating whether ShowProjectSummaryTask is set or not. |
| [SplitsInProgressTasks](../../aspose.tasks/project/splitsinprogresstasks/) { get; set; } | Gets or sets a value indicating whether SplitsInProgressTasks is set or not. |
| [SpreadActualCost](../../aspose.tasks/project/spreadactualcost/) { get; set; } | Gets or sets a value indicating whether SpreadActualCost is set or not. |
| [SpreadPercentComplete](../../aspose.tasks/project/spreadpercentcomplete/) { get; set; } | Gets or sets a value indicating whether SpreadPercentComplete is set or not. |
| [StartDate](../../aspose.tasks/project/startdate/) { get; set; } | Gets or sets a value of StartDate. |
| [StatusDate](../../aspose.tasks/project/statusdate/) { get; set; } | Gets or sets a value of StatusDate. |
| [Subject](../../aspose.tasks/project/subject/) { get; set; } | Gets or sets a value of Subject. |
| [Tables](../../aspose.tasks/project/tables/) { get; } | Gets a list of [`Table`](../table/) objects. |
| [TaskFilters](../../aspose.tasks/project/taskfilters/) { get; } | Gets all the task-based filter definitions. TaskFilters is a collection of [`Filter`](../filter/) objects. |
| [TaskGroups](../../aspose.tasks/project/taskgroups/) { get; } | Gets all the task-based group definitions. TaskGroups is a collection of [`Group`](../group/) objects. |
| [TaskLinks](../../aspose.tasks/project/tasklinks/) { get; } | Gets [`TaskLinkCollection`](../tasklinkcollection/) object. |
| [TaskUpdatesResource](../../aspose.tasks/project/taskupdatesresource/) { get; set; } | Gets or sets a value indicating whether TaskUpdatesResource is set or not. |
| [Template](../../aspose.tasks/project/template/) { get; set; } | Gets or sets a value of Template. |
| [TimescaleFinish](../../aspose.tasks/project/timescalefinish/) { get; set; } | Gets or sets a value of TimescaleFinish. |
| [TimescaleStart](../../aspose.tasks/project/timescalestart/) { get; set; } | Gets or sets a value of TimescaleStart. |
| [Title](../../aspose.tasks/project/title/) { get; set; } | Gets or sets a value of Title. |
| [Uid](../../aspose.tasks/project/uid/) { get; set; } | Gets or sets a value of Uid. |
| [UpdateManuallyScheduledTasksWhenEditingLinks](../../aspose.tasks/project/updatemanuallyscheduledtaskswheneditinglinks/) { get; set; } | Gets or sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |
| [VbaProject](../../aspose.tasks/project/vbaproject/) { get; } | Gets an instance of [`VbaProject`](./vbaproject/) class. |
| [Views](../../aspose.tasks/project/views/) { get; } | Gets a list of [`View`](../view/) objects. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition/) { get; set; } | Gets or sets WBS Code Definition for the project. |
| [WeekStartDay](../../aspose.tasks/project/weekstartday/) { get; set; } | Gets or sets a value of WeekStartDay. |
| [WorkFormat](../../aspose.tasks/project/workformat/) { get; set; } | Gets or sets a value of WorkFormat. |

## Methods

| Name | Description |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto)(Project) | Copies project's main data and properties to another project. |
| [CopyTo](../../aspose.tasks/project/copyto/#copyto_1)(Project, CopyToOptions) | Copies project's main data and properties to another project. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks/)() | Recursively enumerates all project's tasks including root task. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get/)(Key&lt;T, PrjKey&gt;) | Returns the value to which the property is mapped in this container. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime/)(BaselineType) | Returns the baseline save time. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration)(double) | Gets [`Duration`](../duration/) object with the specified number of units and default duration format which is defined in project's settings [`DurationFormat`](../prj/durationformat/). |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_1)(double, TimeUnitType) | Gets [`Duration`](../duration/) object with the specified number of [`TimeUnitType`](../timeunittype/) units. |
| [GetDuration](../../aspose.tasks/project/getduration/#getduration_2)(TimeSpan, TimeUnitType) | Gets [`Duration`](../duration/) object with the specified TimeSpan value and specified [`TimeUnitType`](../timeunittype/) value. |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount)() | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale/)(Days). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_4)(PresentationFormat) | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale/)(Days) and given [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_1)(SaveOptions) | Returns page count for the project to be rendered using given [`SaveOptions`](../../aspose.tasks.saving/saveoptions/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_6)(Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_2)(PageSize, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale/) and [`PageSize`](../../aspose.tasks.visualization/pagesize/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_5)(PresentationFormat, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale/) and [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/). |
| [GetPageCount](../../aspose.tasks/project/getpagecount/#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale/), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) and date range. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors/)(Task) | Returns a collection of task links which are predecessors of the specified task. |
| [GetWork](../../aspose.tasks/project/getwork/)(double) | Gets [`Duration`](../duration/) object with the specified Double value and default work format. |
| [Print](../../aspose.tasks/project/print/#print)() | Prints project to the default printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_2)(PrinterSettings) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_1)(PrintOptions) | Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_6)(string) | Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_3)(PrinterSettings, PrintOptions) | Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_5)(PrinterSettings, string) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print/#print_4)(PrinterSettings, PrintOptions, string) | Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate)() | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields. |
| [Recalculate](../../aspose.tasks/project/recalculate/#recalculate_1)(bool) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields/)() | Recalculates Id, Start and Finish of resources. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish/)() | Recalculates Start and Finish of resources. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments/)() | Eliminates invalid resource assignments from the project resource assignments list. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode)() | Renumber WBS code of all tasks. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode/#renumberwbscode_1)(List&lt;int&gt;) | Renumber WBS code of passed tasks. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter)(DateTime) | Reschedules uncompleted project work to start after a specified date. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter/#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Reschedules uncompleted work for a specified list of tasks to start after a specified date. |
| [Save](../../aspose.tasks/project/save/#save_2)(string) | Saves the project data to the file in mpp format. |
| [Save](../../aspose.tasks/project/save/#save)(Stream, SaveFileFormat) | Saves the project data to the stream. |
| [Save](../../aspose.tasks/project/save/#save_1)(Stream, SimpleSaveOptions) | Saves the project to a stream using the specified save options. |
| [Save](../../aspose.tasks/project/save/#save_3)(string, SaveFileFormat) | Saves the project data to the file. |
| [Save](../../aspose.tasks/project/save/#save_4)(string, SimpleSaveOptions) | Saves the document to a file using the specified save options. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate)(Stream) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_2)(string) | Saves the project as a template to the specified file path. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_1)(Stream, SaveTemplateOptions) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate/#saveastemplate_3)(string, SaveTemplateOptions) | Saves the project as a template. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport)(Stream) | Saves the project overview report to the stream. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_2)(string) | Saves the project overview report to PDF file. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_1)(Stream, ReportType) | Saves the project report of the specified type to the specified stream. |
| [SaveReport](../../aspose.tasks/project/savereport/#savereport_3)(string, ReportType) | Saves the project report of the specified type in PDF format to the specified file path. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks/)() | Recursively collects all child tasks of the root task. |
| [Set](../../aspose.tasks/project/set/#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Maps the specified property to the specified value in this container. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set/#set_1)(Key&lt;T, PrjKey&gt;, T) | Maps the specified property to the specified value in this container. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline)(BaselineType) | Saves baseline fields to the specified baseline for the entire project. |
| [SetBaseline](../../aspose.tasks/project/setbaseline/#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Saves baseline fields to the specified baseline for the selected tasks. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime/)(BaselineType, DateTime) | Sets the baseline save time. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete)(DateTime, bool) | Updates all work as complete through a specified date for the entire project. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete/#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Updates all work as complete through a specified date for the specified list of tasks. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo)(Stream) | Gets project file info from the stream. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo/#getprojectfileinfo_1)(string) | Read project file info from the file. |

## Remarks

The **Project** is a central class in the Aspose.Tasks library.

One can use **Project** to read one of supported project management formats: MPP, MPT, MPX, XML.

To load an existing document in any of the supported formats, pass a file name or a stream into one of the **Project** constructors. To create a blank project, call the parameterless constructor.

Use one of the Save method overloads to save the project in any of the [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/) formats: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

The **Project** stores project-wide information such as [`Views`](./views/), [`BuiltInProps`](./builtinprops/), [`CustomProps`](./customprops/), and [`ExtendedAttributes`](./extendedattributes/). Most of these objects are accessible via the corresponding properties of the **Project** class.

The **Project** is a root entity that contains entry points to manipulate other project entities, such as [`Task`](../task/), [`Resource`](../resource/), [`ResourceAssignment`](../resourceassignment/), [`ExtendedAttribute`](../extendedattribute/) and [`Calendar`](../calendar/).

The **Project** entities can be accessed via typed collections, for example [`Children`](../task/children/), [`Resources`](./resources/), [`ResourceAssignments`](./resourceassignments/), etc.

## Examples

Shows how to work with a &lt;see cref="Aspose.Tasks.Project"/&gt; instance.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Hour); // set the desired project properties
project.Set(Prj.NewTasksAreManual, false);

// adding new tasks and set desired properties
var task1 = project.RootTask.Children.Add("Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 2, 5, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task1.Set(Tsk.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Start, new DateTime(2020, 2, 6, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
task2.Set(Tsk.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// adding new resources
var workResource = project.Resources.Add("Work Resource");
workResource.Set(Rsc.Type, ResourceType.Work);
var costResource = project.Resources.Add("Cost Resource");
costResource.Set(Rsc.Type, ResourceType.Cost);

// adding new resource assignments
var workResourceAssignment = project.ResourceAssignments.Add(task1, workResource);
workResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 5, 8, 0, 0));
workResourceAssignment.Set(Asn.Work, project.GetWork(8));
workResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 5, 17, 0, 0));
var costResourceAssignment = project.ResourceAssignments.Add(task2, costResource);
costResourceAssignment.Set(Asn.Start, new DateTime(2020, 2, 6, 8, 0, 0));
costResourceAssignment.Set(Asn.Work, project.GetWork(8));
costResourceAssignment.Set(Asn.Finish, new DateTime(2020, 2, 6, 17, 0, 0));

// save project in the one of available formats
// here we are saving it in Microsoft Project XML file format.
project.Save(OutDir + "ProjectCreation_out.xml", SaveFileFormat.Xml);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


