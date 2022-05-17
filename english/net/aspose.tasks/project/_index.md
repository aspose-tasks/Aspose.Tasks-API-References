---
title: Project
second_title: Aspose.Tasks for .NET API Reference
description: 
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
| [Project](project)() | Initializes a new instance of the [`Project`](../project) class. |
| [Project](project)(DbSettings) | Initializes a new instance of the [`Project`](../project) class to read data from a database which is specified by the instance of the [`DbSettings`](../../aspose.tasks.connectivity/dbsettings) class. |
| [Project](project)(Stream) | Initializes a new instance of the [`Project`](../project) class from a stream. |
| [Project](project)(StreamReader) | Initializes a new instance of the [`Project`](../project) class from a StreamReader instance. |
| [Project](project)(string) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file). |
| [Project](project)(Stream, LoadOptions) | Initializes a new instance of the [`Project`](../project) class from the Stream with the specified instance of the [`LoadOptions`](../loadoptions) class. |
| [Project](project)(Stream, ParseErrorCallback) | Initializes a new instance of the [`Project`](../project) class from a template(existent mpp or mpt file). |
| [Project](project)(Stream, PrimaveraReadOptions) | Initializes a new instance of the [`Project`](../project) class from the Stream with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project)(Stream, string) | Initializes a new instance of the [`Project`](../project) class from a template(existent mpp or mpt file). |
| [Project](project)(string, LoadOptions) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file) with the specified instance of the [`LoadOptions`](../loadoptions) class. |
| [Project](project)(string, ParseErrorCallback) | Initializes a new instance of the [`Project`](../project) class from a template (existent mpp or mpt file). |
| [Project](project)(string, PrimaveraReadOptions) | Initializes a new instance of the [`Project`](../project) class from a template (existent MPP or MPT file) with the specified instance of the [`PrimaveraReadOptions`](../primaverareadoptions) class. |
| [Project](project)(string, string) | Initializes a new instance of the [`Project`](../project) class from a password protected template (existent mpp or mpt file). |

## Properties

| Name | Description |
| --- | --- |
| [BuiltInProps](builtinprops) { get; } | Gets project's built-in properties collection. |
| [CalculationMode](calculationmode) { get; set; } | Gets or sets calculation mode of a project. Can be one of the values of [`CalculationMode`](./calculationmode) enumeration. |
| [Calendars](calendars) { get; } | Gets [`CalendarCollection`](../calendarcollection) object of this Project instance. |
| [CriticalPath](criticalpath) { get; } | Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. This is an O(n) operation, where n is the number of tasks in the project. |
| [CustomProps](customprops) { get; } | Gets project's custom properties collection. |
| [DefaultView](defaultview) { get; set; } | Gets or sets default view of the project. |
| [DefaultWeekWorkingDays](defaultweekworkingdays) { get; } | Gets the instance of [`WeekDayCollection`](../weekdaycollection) class which represents a collection of project default week working days and working times. |
| [DisplayOptions](displayoptions) { get; } | Gets an instance of the [`ProjectDisplayOptions`](../projectdisplayoptions) class. |
| [ExtendedAttributes](extendedattributes) { get; } | Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project. |
| [OleObjects](oleobjects) { get; } | Gets a collection containing the instances of the [`OleObject`](../oleobject) class which are linked or embedded to this project file. Available for mpp file format only. This collection is read-only except for 'Clear' operation. |
| [OutlineCodes](outlinecodes) { get; } | Gets OutlineCodeDefinitionCollection object. The collection of outline code definitions associated with a project. |
| [ResourceAssignments](resourceassignments) { get; } | Gets ResourceAssignmentCollection object. |
| [ResourceFilters](resourcefilters) { get; } | Gets all the resource-based filter definitions. ResourceFilters is a collection of [`Filter`](../filter) objects. |
| [ResourceGroups](resourcegroups) { get; } | Gets all of the resource-based group definitions. ResourceGroups is a collection of [`Group`](../group) objects. |
| [Resources](resources) { get; } | Gets ResourceCollection object. |
| [RootTask](roottask) { get; } | Gets the root of the tree of tasks. |
| [Tables](tables) { get; } | Gets a list of [`Table`](../table) objects. |
| [TaskFilters](taskfilters) { get; } | Gets all the task-based filter definitions. TaskFilters is a collection of [`Filter`](../filter) objects. |
| [TaskGroups](taskgroups) { get; } | Gets all the task-based group definitions. TaskGroups is a collection of [`Group`](../group) objects. |
| [TaskLinks](tasklinks) { get; } | Gets [`TaskLinkCollection`](../tasklinkcollection) object. |
| [VbaProject](vbaproject) { get; } | Gets an instance of [`VbaProject`](./vbaproject) class. |
| [Views](views) { get; } | Gets a list of [`View`](../view) objects. |
| [WBSCodeDefinition](wbscodedefinition) { get; set; } | Gets or sets WBS Code Definition for the project. |

## Methods

| Name | Description |
| --- | --- |
| [CopyTo](copyto)(Project) | Copies project's main data and properties to another project. |
| [CopyTo](copyto)(Project, CopyToOptions) | Copies project's main data and properties to another project. |
| [EnumerateAllChildTasks](enumerateallchildtasks)() | Recursively enumerates all project's tasks including root task. |
| [Get&lt;T&gt;](get)(Key&lt;T, PrjKey&gt;) | Returns the value to which the property is mapped in this container. |
| [GetBaselineSaveTime](getbaselinesavetime)(BaselineType) | Returns the baseline save time. |
| [GetDuration](getduration)(double) | Gets [`Duration`](../duration) object with the specified number of units and default duration format which is defined in project's settings [`DurationFormat`](../prj/durationformat). |
| [GetDuration](getduration)(double, TimeUnitType) | Gets [`Duration`](../duration) object with the specified number of [`TimeUnitType`](../timeunittype) units. |
| [GetDuration](getduration)(TimeSpan, TimeUnitType) | Gets [`Duration`](../duration) object with the specified TimeSpan value and specified [`TimeUnitType`](../timeunittype) value. |
| [GetPageCount](getpagecount)() | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale)(Days). |
| [GetPageCount](getpagecount)(PresentationFormat) | Returns page count for the project to be rendered using default [`Timescale`](../../aspose.tasks.visualization/timescale)(Days) and given [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) |
| [GetPageCount](getpagecount)(SaveOptions) | Returns page count for the project to be rendered using given [`SaveOptions`](../../aspose.tasks.saving/saveoptions). |
| [GetPageCount](getpagecount)(Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale). |
| [GetPageCount](getpagecount)(PageSize, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale) and [`PageSize`](../../aspose.tasks.visualization/pagesize). |
| [GetPageCount](getpagecount)(PresentationFormat, Timescale) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale) and [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat). |
| [GetPageCount](getpagecount)(PageSize, Timescale, DateTime, DateTime) | Returns page count for the project to be rendered using given [`Timescale`](../../aspose.tasks.visualization/timescale), [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) and date range. |
| [GetPredecessors](getpredecessors)(Task) | Returns a collection of task links which are predecessors of the specified task. |
| [GetWork](getwork)(double) | Gets [`Duration`](../duration) object with the specified Double value and default work format. |
| [Print](print)() | Prints project to the default printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](print)(PrinterSettings) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](print)(PrintOptions) | Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](print)(string) | Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller. |
| [Print](print)(PrinterSettings, PrintOptions) | Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller. |
| [Print](print)(PrinterSettings, string) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [Print](print)(PrinterSettings, PrintOptions, string) | Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller. |
| [Recalculate](recalculate)() | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields. |
| [Recalculate](recalculate)(bool) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation. |
| [RecalculateResourceFields](recalculateresourcefields)() | Recalculates Id, Start and Finish of resources. |
| [RecalculateResourceStartFinish](recalculateresourcestartfinish)() | Recalculates Start and Finish of resources. |
| [RemoveInvalidResourceAssignments](removeinvalidresourceassignments)() | Eliminates invalid resource assignments from the project resource assignments list. |
| [RenumberWBSCode](renumberwbscode)() | Renumber WBS code of all tasks. |
| [RenumberWBSCode](renumberwbscode)(List&lt;int&gt;) | Renumber WBS code of passed tasks. |
| [RescheduleUncompletedWorkToStartAfter](rescheduleuncompletedworktostartafter)(DateTime) | Reschedules uncompleted project work to start after a specified date. |
| [RescheduleUncompletedWorkToStartAfter](rescheduleuncompletedworktostartafter)(DateTime, List&lt;Task&gt;) | Reschedules uncompleted work for a specified list of tasks to start after a specified date. |
| [Save](save)(string) | Saves the project data to the file in mpp format. |
| [Save](save)(Stream, MPPSaveOptions) | Saves the project to a stream using the specified save options. |
| [Save](save)(Stream, SaveFileFormat) | Saves the project data to the stream. |
| [Save](save)(Stream, SaveOptions) | Saves the project to a stream using the specified save options. |
| [Save](save)(string, MPPSaveOptions) | Saves the document to mpp file format using the specified save options. |
| [Save](save)(string, SaveFileFormat) | Saves the project data to the file. |
| [Save](save)(string, SaveOptions) | Saves the document to a file using the specified save options. |
| [SaveAsTemplate](saveastemplate)(Stream) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](saveastemplate)(string) | Saves the project as a template to the specified file path. |
| [SaveAsTemplate](saveastemplate)(Stream, SaveTemplateOptions) | Saves the project as a template to a specified stream. |
| [SaveAsTemplate](saveastemplate)(string, SaveTemplateOptions) | Saves the project as a template. |
| [SaveReport](savereport)(Stream) | Saves the project overview report to the stream. |
| [SaveReport](savereport)(string) | Saves the project overview report to PDF file. |
| [SaveReport](savereport)(Stream, ReportType) | Saves the project report of the specified type to the specified stream. |
| [SaveReport](savereport)(string, ReportType) | Saves the project report of the specified type in PDF format to the specified file path. |
| [SelectAllChildTasks](selectallchildtasks)() | Recursively collects all child tasks of the root task. |
| [Set](set)(Key&lt;DateTime, PrjKey&gt;, DateTime) | Maps the specified property to the specified value in this container. |
| [Set&lt;T&gt;](set)(Key&lt;T, PrjKey&gt;, T) | Maps the specified property to the specified value in this container. |
| [SetBaseline](setbaseline)(BaselineType) | Saves baseline fields to the specified baseline for the entire project. |
| [SetBaseline](setbaseline)(BaselineType, IEnumerable&lt;Task&gt;) | Saves baseline fields to the specified baseline for the selected tasks. |
| [SetBaselineSaveTime](setbaselinesavetime)(BaselineType, DateTime) | Sets the baseline save time. |
| [UpdateProjectWorkAsComplete](updateprojectworkascomplete)(DateTime, bool) | Updates all work as complete through a specified date for the entire project. |
| [UpdateProjectWorkAsComplete](updateprojectworkascomplete)(DateTime, bool, List&lt;Task&gt;) | Updates all work as complete through a specified date for the specified list of tasks. |
| static [GetProjectFileInfo](getprojectfileinfo)(Stream) | Gets project file info from the stream. |
| static [GetProjectFileInfo](getprojectfileinfo)(string) | Read project file info from the file. |

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
