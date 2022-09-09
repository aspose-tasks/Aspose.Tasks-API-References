---
title: Project
second_title: Aspose.Tasks for .NET API Reference
description: Represents a project.
type: docs
weight: 1180
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
| [Project](project#constructor)() | Initializes a new instance of the [`Project`](../project) class. |
| [Project](project#constructor_1)(DbSettings) | Initializes a new instance of the [`Project`](../project) class to read data from a database which is specified by the instance of the [`DbSettings`](../../aspose.tasks.connectivity/dbsettings) class. |
| [Project](project#constructor_2)(Stream) | Initializes a new instance of the [`Project`](../project) class from a stream. |
| [Project](project#constructor_9)(StreamReader) | Initializes a new instance of the [`Project`](../project) class from a StreamReader instance. |
| [Project](project#constructor_10)(string) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file). |
| [Project](project#constructor_3)(Stream, LoadOptions) | Initializes a new instance of the [`Project`](../project) class from the Stream with the specified instance of the [`LoadOptions`](../loadoptions) class. |
| [Project](project#constructor_4)(Stream, ParseErrorCallback) | Initializes a new instance of the [`Project`](../project) class from a template(existent mpp or mpt file). |
| [Project](project#constructor_6)(Stream, PrimaveraReadOptions) | Initializes a new instance of the [`Project`](../project) class from the Stream with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project#constructor_8)(Stream, string) | Initializes a new instance of the [`Project`](../project) class from a template(existent mpp or mpt file). |
| [Project](project#constructor_11)(string, LoadOptions) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file) with the specified instance of the [`LoadOptions`](../loadoptions) class. |
| [Project](project#constructor_12)(string, ParseErrorCallback) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file). |
| [Project](project#constructor_14)(string, PrimaveraReadOptions) | Initializes a new instance of the [`Project`](../project) class from a template (existent MPP or MPT file) with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project#constructor_16)(string, string) | Initializes a new instance of the [`Project`](../project) class from a password protected template (existent mpp or mpt file). |

## Properties

| Name | Description |
| --- | --- |
| [BuiltInProps](../../aspose.tasks/project/builtinprops) { get; } | Gets project's built-in properties collection. |
| [CalculationMode](../../aspose.tasks/project/calculationmode) { get; set; } | Gets or sets calculation mode of a project. Can be one of the values of [`CalculationMode`](./calculationmode) enumeration. |
| [Calendars](../../aspose.tasks/project/calendars) { get; } | Gets [`CalendarCollection`](../calendarcollection) object of this Project instance. |
| [CriticalPath](../../aspose.tasks/project/criticalpath) { get; } | Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. This is an O(n) operation, where n is the number of tasks in the project. |
| [CustomProps](../../aspose.tasks/project/customprops) { get; } | Gets project's custom properties collection. |
| [DefaultView](../../aspose.tasks/project/defaultview) { get; set; } | Gets or sets default view of the project. |
| [DefaultWeekWorkingDays](../../aspose.tasks/project/defaultweekworkingdays) { get; } | Gets the instance of [`WeekDayCollection`](../weekdaycollection) class which represents a collection of project default week working days and working times. |
| [DisplayOptions](../../aspose.tasks/project/displayoptions) { get; } | Gets an instance of the [`ProjectDisplayOptions`](../projectdisplayoptions) class. |
| [ExtendedAttributes](../../aspose.tasks/project/extendedattributes) { get; } | Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project. |
| [OleObjects](../../aspose.tasks/project/oleobjects) { get; } | Gets a collection containing the instances of the [`OleObject`](../oleobject) class which are linked or embedded to this project file. Available for mpp file format only. This collection is read-only except for 'Clear' operation. |
| [OutlineCodes](../../aspose.tasks/project/outlinecodes) { get; } | Gets OutlineCodeDefinitionCollection object. The collection of outline code definitions associated with a project. |
| [ResourceAssignments](../../aspose.tasks/project/resourceassignments) { get; } | Gets ResourceAssignmentCollection object. |
| [ResourceFilters](../../aspose.tasks/project/resourcefilters) { get; } | Gets all the resource-based filter definitions. ResourceFilters is a collection of [`Filter`](../filter) objects. |
| [ResourceGroups](../../aspose.tasks/project/resourcegroups) { get; } | Gets all of the resource-based group definitions. ResourceGroups is a collection of [`Group`](../group) objects. |
| [Resources](../../aspose.tasks/project/resources) { get; } | Gets ResourceCollection object. |
| [RootTask](../../aspose.tasks/project/roottask) { get; } | Gets the root of the tree of tasks. |
| [Tables](../../aspose.tasks/project/tables) { get; } | Gets a list of [`Table`](../table) objects. |
| [TaskFilters](../../aspose.tasks/project/taskfilters) { get; } | Gets all the task-based filter definitions. TaskFilters is a collection of [`Filter`](../filter) objects. |
| [TaskGroups](../../aspose.tasks/project/taskgroups) { get; } | Gets all the task-based group definitions. TaskGroups is a collection of [`Group`](../group) objects. |
| [TaskLinks](../../aspose.tasks/project/tasklinks) { get; } | Gets [`TaskLinkCollection`](../tasklinkcollection) object. |
| [VbaProject](../../aspose.tasks/project/vbaproject) { get; } | Gets an instance of [`VbaProject`](./vbaproject) class. |
| [Views](../../aspose.tasks/project/views) { get; } | Gets a list of [`View`](../view) objects. |
| [WBSCodeDefinition](../../aspose.tasks/project/wbscodedefinition) { get; set; } | Gets or sets WBS Code Definition for the project. |

## Methods

| Name | Description |
| --- | --- |
| [CopyTo](../../aspose.tasks/project/copyto#copyto)(Project) | Copies project's main data and properties to another project. |
| [CopyTo](../../aspose.tasks/project/copyto#copyto_1)(Project, CopyToOptions) | Copies project's main data and properties to another project. |
| [EnumerateAllChildTasks](../../aspose.tasks/project/enumerateallchildtasks)() | Recursively enumerates all project's tasks including root task. |
| [Get&lt;T&gt;](../../aspose.tasks/project/get)(Key&lt;T, PrjKey&gt;) | Returns the value to which the property is mapped in this container. |
| [GetBaselineSaveTime](../../aspose.tasks/project/getbaselinesavetime)(BaselineType) | Returns the baseline save time. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration)(double) | Gets [`Duration`](../duration) object with the specified number of units and default duration format which is defined in project's settings [`DurationFormat`](../prj/durationformat). |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_1)(double, TimeUnitType) | Gets [`Duration`](../duration) object with the specified number of [`TimeUnitType`](../timeunittype) units. |
| [GetDuration](../../aspose.tasks/project/getduration#getduration_2)(TimeSpan, TimeUnitType) | Gets [`Duration`](../duration) object with the specified TimeSpan value and specified [`TimeUnitType`](../timeunittype) value. |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount)() | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale)(Days). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_4)(PresentationFormat) | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale)(Days) and given [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_1)(SaveOptions) | Returns page count for the project to be rendered using given [`SaveOptions`](../../aspose.tasks.saving/saveoptions). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_6)(Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_2)(PageSize, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale) and [`PageSize`](../../aspose.tasks.visualization/pagesize). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_5)(PresentationFormat, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale) and [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat). |
| [GetPageCount](../../aspose.tasks/project/getpagecount#getpagecount_3)(PageSize, Timescale, DateTime, DateTime) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) and date range. |
| [GetPredecessors](../../aspose.tasks/project/getpredecessors)(Task) | Returns a collection of task links which are predecessors of the specified task. |
| [GetWork](../../aspose.tasks/project/getwork)(double) | Gets [`Duration`](../duration) object with the specified Double value and default work format. |
| [Print](../../aspose.tasks/project/print#print)() | Prints project to the default printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_2)(PrinterSettings) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_1)(PrintOptions) | Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_6)(string) | Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_3)(PrinterSettings, PrintOptions) | Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_5)(PrinterSettings, string) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](../../aspose.tasks/project/print#print_4)(PrinterSettings, PrintOptions, string) | Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate)() | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields. |
| [Recalculate](../../aspose.tasks/project/recalculate#recalculate_1)(bool) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation. |
| [RecalculateResourceFields](../../aspose.tasks/project/recalculateresourcefields)() | Recalculates Id, Start and Finish of resources. |
| [RecalculateResourceStartFinish](../../aspose.tasks/project/recalculateresourcestartfinish)() | Recalculates Start and Finish of resources. |
| [RemoveInvalidResourceAssignments](../../aspose.tasks/project/removeinvalidresourceassignments)() | Eliminates invalid resource assignments from the project resource assignments list. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode)() | Renumber WBS code of all tasks. |
| [RenumberWBSCode](../../aspose.tasks/project/renumberwbscode#renumberwbscode_1)(List&lt;int&gt;) | Renumber WBS code of passed tasks. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter)(DateTime) | Reschedules uncompleted project work to start after a specified date. |
| [RescheduleUncompletedWorkToStartAfter](../../aspose.tasks/project/rescheduleuncompletedworktostartafter#rescheduleuncompletedworktostartafter_1)(DateTime, List&lt;Task&gt;) | Reschedules uncompleted work for a specified list of tasks to start after a specified date. |
| [Save](../../aspose.tasks/project/save#save_3)(string) | Saves the project data to the file in mpp format. |
| [Save](../../aspose.tasks/project/save#save)(Stream, MPPSaveOptions) | Saves the project to a stream using the specified save options. |
| [Save](../../aspose.tasks/project/save#save_1)(Stream, SaveFileFormat) | Saves the project data to the stream. |
| [Save](../../aspose.tasks/project/save#save_2)(Stream, SaveOptions) | Saves the project to a stream using the specified save options. |
| [Save](../../aspose.tasks/project/save#save_4)(string, MPPSaveOptions) | Saves the document to mpp file format using the specified save options. |
| [Save](../../aspose.tasks/project/save#save_5)(string, SaveFileFormat) | Saves the project data to the file. |
| [Save](../../aspose.tasks/project/save#save_6)(string, SaveOptions) | Saves the document to a file using the specified save options. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate)(Stream) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_2)(string) | Saves the project as a template to the specified file path. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_1)(Stream, SaveTemplateOptions) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](../../aspose.tasks/project/saveastemplate#saveastemplate_3)(string, SaveTemplateOptions) | Saves the project as a template. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport)(Stream) | Saves the project overview report to the stream. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_2)(string) | Saves the project overview report to PDF file. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_1)(Stream, ReportType) | Saves the project report of the specified type to the specified stream. |
| [SaveReport](../../aspose.tasks/project/savereport#savereport_3)(string, ReportType) | Saves the project report of the specified type in PDF format to the specified file path. |
| [SelectAllChildTasks](../../aspose.tasks/project/selectallchildtasks)() | Recursively collects all child tasks of the root task. |
| [Set](../../aspose.tasks/project/set#set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Maps the specified property to the specified value in this container. |
| [Set&lt;T&gt;](../../aspose.tasks/project/set#set_1)(Key&lt;T, PrjKey&gt;, T) | Maps the specified property to the specified value in this container. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline)(BaselineType) | Saves baseline fields to the specified baseline for the entire project. |
| [SetBaseline](../../aspose.tasks/project/setbaseline#setbaseline_1)(BaselineType, IEnumerable&lt;Task&gt;) | Saves baseline fields to the specified baseline for the selected tasks. |
| [SetBaselineSaveTime](../../aspose.tasks/project/setbaselinesavetime)(BaselineType, DateTime) | Sets the baseline save time. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete)(DateTime, bool) | Updates all work as complete through a specified date for the entire project. |
| [UpdateProjectWorkAsComplete](../../aspose.tasks/project/updateprojectworkascomplete#updateprojectworkascomplete_1)(DateTime, bool, List&lt;Task&gt;) | Updates all work as complete through a specified date for the specified list of tasks. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo)(Stream) | Gets project file info from the stream. |
| static [GetProjectFileInfo](../../aspose.tasks/project/getprojectfileinfo#getprojectfileinfo_1)(string) | Read project file info from the file. |

### Remarks

The **Project** is a central class in the Aspose.Tasks library.

One can use **Project** to read one of supported project management formats: MPP, MPT, MPX, XML.

To load an existing document in any of the supported formats, pass a file name or a stream into one of the **Project** constructors. To create a blank project, call the parameterless constructor.

Use one of the Save method overloads to save the project in any of the [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat) formats: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

To print the project, use one of the [`Print`](./print) method overloads.

The **Project** stores project-wide information such as [`Views`](./views), [`BuiltInProps`](./builtinprops), [`CustomProps`](./customprops), and [`ExtendedAttributes`](./extendedattributes). Most of these objects are accessible via the corresponding properties of the **Project** class.

The **Project** is a root entity that contains entry points to manipulate other project entities, such as [`Task`](../task), [`Resource`](../resource), [`ResourceAssignment`](../resourceassignment), [`ExtendedAttribute`](../extendedattribute) and [`Calendar`](../calendar).

The **Project** entities can be accessed via typed collections, for example [`Children`](../task/children), [`Resources`](./resources), [`ResourceAssignments`](./resourceassignments), etc.

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
