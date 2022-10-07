---
title: Project
second_title: Aspose.Tasks for Java API Reference
description: Represents a project.
type: docs
weight: 196
url: /java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Integer>
```

Represents a project.

--------------------

The **Project** is a central class in the Aspose.Tasks library.

One can use **Project** to read one of supported project management formats: MPP, MPT, MPX, XML.

To load an existing document in any of the supported formats, pass a file name or a stream into one of the **Project** constructors. To create a blank project, call the parameterless constructor.

Use one of the Save method overloads to save the project in any of the [SaveFileFormat](../../com.aspose.tasks/savefileformat) formats: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

To print the project, use one of the [print()](../../com.aspose.tasks/project\#print--) method overloads.

The **Project** stores project-wide information such as  Aspose.Tasks.Project.Views ([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-)),  Aspose.Tasks.Project.BuiltInProps ([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-)),  Aspose.Tasks.Project.CustomProps ([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)), and  Aspose.Tasks.Project.ExtendedAttributes ([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-)). Most of these objects are accessible via the corresponding properties of the **Project** class.

The **Project** is a root entity that contains entry points to manipulate other project entities, such as [Task](../../com.aspose.tasks/task), [Resource](../../com.aspose.tasks/resource), [ResourceAssignment](../../com.aspose.tasks/resourceassignment), [ExtendedAttribute](../../com.aspose.tasks/extendedattribute) and [Calendar](../../com.aspose.tasks/calendar).

The **Project** entities can be accessed via typed collections, for example  Aspose.Tasks.Task.Children ([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-)),  Aspose.Tasks.Project.Resources ([getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-)),  Aspose.Tasks.Project.ResourceAssignments ([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-)), etc.
## Constructors

| Constructor | Description |
| --- | --- |
| [Project()](#Project--) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class. |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a password protected template (existent mpp or mpt file). |
| [Project(String projectTemplate)](#Project-java.lang.String-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file). |
| [Project(InputStream stream, PrimaveraXmlReadingOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraXmlReadingOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-com.aspose.tasks.PrimaveraXmlReadingOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file). |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a stream. |
| [Project(String projectTemplate, PrimaveraXmlReadingOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraXmlReadingOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent MPP or MPT file) with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent MPP or MPT file) with the specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-com.aspose.tasks.PrimaveraXmlReadingOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file) with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class to read data from a database which is specified by the instance of the [DbSettings](../../com.aspose.tasks/dbsettings) class. |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template(existent mpp or mpt file). |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template(existent mpp or mpt file). |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file) with the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions) class. |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions) class. |
## Methods

| Method | Description |
| --- | --- |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | Copies project's main data and properties to another project. |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | Copies project's main data and properties to another project. |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | Recursively enumerates all project's tasks including root task. |
| [&lt;T&gt;get(Key&lt;T,Integer&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--) | Returns the value to which the property is mapped in this container. |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | Returns the baseline save time. |
| [getBuiltInProps()](#getBuiltInProps--) | Gets project's built-in properties collection. |
| [getCalculationMode()](#getCalculationMode--) | Gets calculation mode of a project. |
| [setCalculationMode(int value)](#setCalculationMode-int-) | Sets calculation mode of a project. |
| [getCalendars()](#getCalendars--) | Gets [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance. |
| [getCriticalPath()](#getCriticalPath--) | Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. |
| [getCustomProps()](#getCustomProps--) | Gets project's custom properties collection. |
| [getDefaultView()](#getDefaultView--) | Gets default view of the project. |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | Sets default view of the project. |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | Gets the instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which represents a collection of project default week working days and working times. |
| [getDisplayOptions()](#getDisplayOptions--) | Gets an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class. |
| [getDuration(double val)](#getDuration-double-) | Gets [Duration](../../com.aspose.tasks/duration) object with the specified number of units and default duration format which is defined in project's settings [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT). |
| [getDuration(double val, int timeUnit)](#getDuration-double-int-) | Gets [Duration](../../com.aspose.tasks/duration) object with the specified number of [TimeUnitType](../../com.aspose.tasks/timeunittype) units. |
| [getExtendedAttributes()](#getExtendedAttributes--) | Gets ExtendedAttributeDefinitionCollection object. |
| [getOleObjects()](#getOleObjects--) | Gets a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file. |
| [getOutlineCodes()](#getOutlineCodes--) | Gets OutlineCodeDefinitionCollection object. |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | Returns page count for the project to be rendered using given [SaveOptions](../../com.aspose.tasks/saveoptions). |
| [getPageCount()](#getPageCount--) | Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days). |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat) |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range. |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize). |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale). |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat). |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | Returns a collection of task links which are predecessors of the specified task. |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | Read project file info from the file. |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | Gets project file info from the stream. |
| [getResourceAssignments()](#getResourceAssignments--) | Gets ResourceAssignmentCollection object. |
| [getResourceFilters()](#getResourceFilters--) | Gets all the resource-based filter definitions. |
| [getResourceGroups()](#getResourceGroups--) | Gets all of the resource-based group definitions. |
| [getResources()](#getResources--) | Gets ResourceCollection object. |
| [getRootTask()](#getRootTask--) | Gets the root of the tree of tasks. |
| [getTables()](#getTables--) | Gets a list of [Table](../../com.aspose.tasks/table) objects. |
| [getTaskFilters()](#getTaskFilters--) | Gets all the task-based filter definitions. |
| [getTaskGroups()](#getTaskGroups--) | Gets all the task-based group definitions. |
| [getTaskLinks()](#getTaskLinks--) | Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object. |
| [getVbaProject()](#getVbaProject--) | Gets an instance of  VbaProject ([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class. |
| [getViews()](#getViews--) | Gets a list of [View](../../com.aspose.tasks/view) objects. |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | Gets WBS Code Definition for the project. |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | Sets WBS Code Definition for the project. |
| [getWork(double val)](#getWork-double-) | Gets [Duration](../../com.aspose.tasks/duration) object with the specified  double  value and default work format. |
| [print()](#print--) | Prints project to the default printer with default printer settings using the standard (no User Interface) print controller. |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller. |
| [print(String printerName)](#print-java.lang.String-) | Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller. |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | Prints project according to the specified printer settings using the standard (no User Interface) print controller. |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller. |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller. |
| [recalculate()](#recalculate--) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields. |
| [recalculate(boolean validate)](#recalculate-boolean-) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation. |
| [recalculateResourceFields()](#recalculateResourceFields--) | Recalculates Id, Start and Finish of resources. |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | Recalculates Start and Finish of resources. |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | Eliminates invalid resource assignments from the project resource assignments list. |
| [renumberWBSCode()](#renumberWBSCode--) | Renumber WBS code of all tasks. |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | Renumber WBS code of passed tasks. |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | Reschedules uncompleted project work to start after a specified date. |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | Reschedules uncompleted work for a specified list of tasks to start after a specified date. |
| [save(String filename, MPPSaveOptions options)](#save-java.lang.String-com.aspose.tasks.MPPSaveOptions-) | Saves the document to mpp file format using the specified save options. |
| [save(String filename, SaveOptions options)](#save-java.lang.String-com.aspose.tasks.SaveOptions-) | Saves the document to a file using the specified save options. |
| [save(String filename, int format)](#save-java.lang.String-int-) | Saves the project data to the file. |
| [save(String filename)](#save-java.lang.String-) | Saves the project data to the file in mpp format. |
| [save(OutputStream stream, SaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SaveOptions-) | Saves the project to a stream using the specified save options. |
| [save(OutputStream stream, MPPSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.MPPSaveOptions-) | Saves the project to a stream using the specified save options. |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | Saves the project data to the stream. |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | Saves the project as a template. |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | Saves the project as a template to the specified file path. |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | Saves the project as a template to a specified stream. |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | Saves the project as a template to a specified stream. |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | Saves the project overview report to the stream. |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | Saves the project overview report to PDF file. |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | Saves the project report of the specified type to the specified stream. |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | Saves the project report of the specified type in PDF format to the specified file path. |
| [selectAllChildTasks()](#selectAllChildTasks--) | Recursively collects all child tasks of the root task. |
| [&lt;T&gt;set(Key&lt;T,Integer&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-) | Maps the specified property to the specified value in this container. |
| [set(Key&lt;Date,Integer&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-) | Maps the specified property to the specified value in this container. |
| [setBaseline(int baselineType)](#setBaseline-int-) | Saves baseline fields to the specified baseline for the entire project. |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | Saves baseline fields to the specified baseline for the selected tasks. |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | Sets the baseline save time. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | Updates all work as complete through a specified date for the entire project. |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | Updates all work as complete through a specified date for the specified list of tasks. |
### Project() {#Project--}
```
public Project()
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class.

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a password protected template (existent mpp or mpt file).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from. |
| protectionPassword | java.lang.String | Protection password.

--------------------

Reading password protected files currently supported for MSP 2003 file format only. |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from. |

### Project(InputStream stream, PrimaveraXmlReadingOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraXmlReadingOptions-}
```
public Project(InputStream stream, PrimaveraXmlReadingOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Stream of the Project java.io.InputStreamclass |
| options | [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) | the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions)class |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-com.aspose.tasks.PrimaveraXmlReadingOptions-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Stream of the Project java.io.InputStreamclass |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | the specified callback method to handle xml parse errors |
| options | [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) | the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions)class |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | the specified callback method to handle xml parse errors. |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream to load a template from. |

### Project(String projectTemplate, PrimaveraXmlReadingOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraXmlReadingOptions-}
```
public Project(String projectTemplate, PrimaveraXmlReadingOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent MPP or MPT file) with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from |
| options | [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) | the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent MPP or MPT file) with the specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | the specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class. |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-com.aspose.tasks.PrimaveraXmlReadingOptions-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler, PrimaveraXmlReadingOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file) with the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | the specified callback method to handle xml parse errors |
| options | [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) | the specified instance of the [PrimaveraXmlReadingOptions](../../com.aspose.tasks/primaveraxmlreadingoptions) class. |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class to read data from a database which is specified by the instance of the [DbSettings](../../com.aspose.tasks/dbsettings) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | the specified instance of the [DbSettings](../../com.aspose.tasks/dbsettings) class. |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template(existent mpp or mpt file).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream to load a template from. |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | the specified callback method to handle xml parse errors. |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template(existent mpp or mpt file).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | java.io.InputStream to load a template from. |
| protectionPassword | java.lang.String | Protection password.

--------------------

Reading password protected files currently supported for MSP 2003 file format only. |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from a template (existent mpp or mpt file) with the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| projectTemplate | java.lang.String | Path to template to create project from |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions) class. |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


Initializes a new instance of the [Project](../../com.aspose.tasks/project) class from the Stream with the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions) class.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | Stream of the Project java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | the specified instance of the [LoadOptions](../../com.aspose.tasks/loadoptions)class |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


Copies project's main data and properties to another project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Another project to copy data to. |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


Copies project's main data and properties to another project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | Another project to copy data to. |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | Copy options to control copy process. |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


Recursively enumerates all project's tasks including root task.

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - IEnumerable which can be used to iterate over all project's tasks.

--------------------

Provides a more lightweight way to iterate over tasks compared to [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) method as it does not allocate memory for all tasks.
### &lt;T&gt;get(Key&lt;T,Integer&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Integer--}
```
public final T <T>get(Key<T,Integer> key)
```


Returns the value to which the property is mapped in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key.

 T : the type of the mapped value. |

**Returns:**
T - the value to which the property is mapped in this container.
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


Returns the baseline save time. Returns DateTime.MinValue (00:00:00.0000000 UTC, 1st January 0001) if the baseline was not saved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |

**Returns:**
java.util.Date - The baseline's last save date and time.
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


Gets project's built-in properties collection.

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


Gets calculation mode of a project. Can be one of the values of  CalculationMode ([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Returns:**
int - calculation mode of a project.
### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of  CalculationMode ([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


Gets [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project.

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

This is an O(n) operation, where n is the number of tasks in the project.
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


Gets project's custom properties collection.

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


Gets default view of the project.

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


Gets the instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which represents a collection of project default week working days and working times.

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

The data contains only in mpp files (not in xml).
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


Gets an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified number of units and default duration format which is defined in project's settings [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified number of units. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, int timeUnit) {#getDuration-double-int-}
```
public final Duration getDuration(double val, int timeUnit)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified number of [TimeUnitType](../../com.aspose.tasks/timeunittype) units.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified number of units. |
| timeUnit | int | specified TimeUnitType value. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project.

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


Gets a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.

--------------------

Available for mpp file format only. This collection is read-only except for 'Clear' operation.

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


Gets OutlineCodeDefinitionCollection object. The collection of outline code definitions associated with a project.

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


Returns page count for the project to be rendered using given [SaveOptions](../../com.aspose.tasks/saveoptions).

--------------------

> ```
> In this example instance of HtmlSaveOptions and the number of pages in resulting HTML is written to the console.
>   ```
> 
>   [C#]
>   Project project = new Project(@"test.mpp");
>   HtmlSaveOptions saveOptions = new HtmlSaveOptions
>   {
>       IncludeProjectNameInPageHeader = false,
>       IncludeProjectNameInTitle = false,
>       PageSize = PageSize.A4,
>       Timescale = Timescale.Days,
>       StartDate = project.Get(Prj.StartDate).Date,
>       EndDate = project.Get(Prj.FinishDate).Date
>   };
>   Console.WriteLine(project.GetPageCount(saveOptions));
>   
> ```
> ```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days).

**Returns:**
int - Page count to be rendered.
### getPageCount_PresentationFormat(int format) {#getPageCount-PresentationFormat-int-}
```
public final int getPageCount_PresentationFormat(int format)
```


Returns page count for the project to be rendered using default [Timescale](../../com.aspose.tasks/timescale)(Days) and given [PresentationFormat](../../com.aspose.tasks/presentationformat)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate) {#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-}
```
public final int getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale), [PresentationFormat](../../com.aspose.tasks/presentationformat) and date range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |
| startDate | java.util.Date | The start date to get page count for. |
| endDate | java.util.Date | The end date to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_PageSize(int pageSize, int scale) {#getPageCount-PageSize-int-int-}
```
public final int getPageCount_PageSize(int pageSize, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PageSize](../../com.aspose.tasks/pagesize).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pageSize | int | [PageSize](../../com.aspose.tasks/pagesize) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount_Timescale(int scale) {#getPageCount-Timescale-int-}
```
public final int getPageCount_Timescale(int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPageCount(int format, int scale) {#getPageCount-int-int-}
```
public final int getPageCount(int format, int scale)
```


Returns page count for the project to be rendered using given [Timescale](../../com.aspose.tasks/timescale) and [PresentationFormat](../../com.aspose.tasks/presentationformat).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | int | [PresentationFormat](../../com.aspose.tasks/presentationformat) to get page count for. |
| scale | int | [Timescale](../../com.aspose.tasks/timescale) to get page count for. |

**Returns:**
int - Page count to be rendered.
### getPredecessors(Task task) {#getPredecessors-com.aspose.tasks.Task-}
```
public final TaskLinkCollection getPredecessors(Task task)
```


Returns a collection of task links which are predecessors of the specified task.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | The task to get predecessors for. |

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - List of predecessors [TaskLink](../../com.aspose.tasks/tasklink).
### getProjectFileInfo(String filename) {#getProjectFileInfo-java.lang.String-}
```
public static ProjectFileInfo getProjectFileInfo(String filename)
```


Read project file info from the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The project filename. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getProjectFileInfo(InputStream stream) {#getProjectFileInfo-java.io.InputStream-}
```
public static ProjectFileInfo getProjectFileInfo(InputStream stream)
```


Gets project file info from the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.InputStream | The data stream. |

**Returns:**
[ProjectFileInfo](../../com.aspose.tasks/projectfileinfo) - The project file info [ProjectFileInfo](../../com.aspose.tasks/projectfileinfo).
### getResourceAssignments() {#getResourceAssignments--}
```
public final ResourceAssignmentCollection getResourceAssignments()
```


Gets ResourceAssignmentCollection object.

**Returns:**
[ResourceAssignmentCollection](../../com.aspose.tasks/resourceassignmentcollection) - ResourceAssignmentCollection object.
### getResourceFilters() {#getResourceFilters--}
```
public final FilterCollection getResourceFilters()
```


Gets all the resource-based filter definitions. ResourceFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the resource-based filter definitions.
### getResourceGroups() {#getResourceGroups--}
```
public final GroupCollection getResourceGroups()
```


Gets all of the resource-based group definitions. ResourceGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all of the resource-based group definitions.
### getResources() {#getResources--}
```
public final ResourceCollection getResources()
```


Gets ResourceCollection object.

**Returns:**
[ResourceCollection](../../com.aspose.tasks/resourcecollection) - ResourceCollection object.
### getRootTask() {#getRootTask--}
```
public final Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getTables() {#getTables--}
```
public final TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
public final FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
public final GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
public final TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getVbaProject() {#getVbaProject--}
```
public final VbaProject getVbaProject()
```


Gets an instance of  VbaProject ([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of  VbaProject ([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
public final ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
public final WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified  double  value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### print() {#print--}
```
public final void print()
```


Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.

### print(PrintOptions options) {#print-com.aspose.tasks.PrintOptions-}
```
public final void print(PrintOptions options)
```


Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

### print(PrinterSettings printerSettings, String documentName) {#print-com.aspose.tasks.PrinterSettings-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, String documentName)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### print(PrinterSettings printerSettings, PrintOptions options) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options)
```


Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |

### print(PrinterSettings printerSettings, PrintOptions options, String documentName) {#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-}
```
public final void print(PrinterSettings printerSettings, PrintOptions options, String documentName)
```


Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |
| options | [PrintOptions](../../com.aspose.tasks/printoptions) | the specified instance of the [PrintOptions](../../com.aspose.tasks/printoptions) class. |
| documentName | java.lang.String | the document name to display (for example, in a print status dialog box or printer queue). |

### recalculate() {#recalculate--}
```
public final void recalculate()
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields.

### recalculate(boolean validate) {#recalculate-boolean-}
```
public final void recalculate(boolean validate)
```


Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validate | boolean | If true the validation of recalculation will be performed. What data is validated: At the moment only basic validation of task and task link date ranges is implemented. Task's date ranges (e.g. ActualStart - ActualFinish, EarlyStart - EarlyFinish, etc.) as well as Task Links dates will be checked against the date criteria that start date is less or equal than finish date. If any of conditions described above is failed then [RecalculationValidationException](../../com.aspose.tasks/recalculationvalidationexception) will be thrown. |

### recalculateResourceFields() {#recalculateResourceFields--}
```
public final void recalculateResourceFields()
```


Recalculates Id, Start and Finish of resources.

### recalculateResourceStartFinish() {#recalculateResourceStartFinish--}
```
public final void recalculateResourceStartFinish()
```


Recalculates Start and Finish of resources.

### removeInvalidResourceAssignments() {#removeInvalidResourceAssignments--}
```
public final void removeInvalidResourceAssignments()
```


Eliminates invalid resource assignments from the project resource assignments list.

--------------------

MS Project creates an empty resource assignment for each task. Call the method to remove them.

### renumberWBSCode() {#renumberWBSCode--}
```
public final void renumberWBSCode()
```


Renumber WBS code of all tasks.

### renumberWBSCode(List&lt;Integer&gt; taskIds) {#renumberWBSCode-java.util.List-java.lang.Integer--}
```
public final void renumberWBSCode(List<Integer> taskIds)
```


Renumber WBS code of passed tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| taskIds | java.util.List&lt;java.lang.Integer&gt; | Task identifiers to renumber WBS codes. |

### rescheduleUncompletedWorkToStartAfter(Date after) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after)
```


Reschedules uncompleted project work to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after.

--------------------

Ensure that Project.CanSplitsInProgressTasks flag is set to true before using this method. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for.

--------------------

Ensure that Project.CanSplitsInProgressTasks flag is set to true before using this method. |

### save(String filename, MPPSaveOptions options) {#save-java.lang.String-com.aspose.tasks.MPPSaveOptions-}
```
public final void save(String filename, MPPSaveOptions options)
```


Saves the document to mpp file format using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) | The save options. |

### save(String filename, SaveOptions options) {#save-java.lang.String-com.aspose.tasks.SaveOptions-}
```
public final void save(String filename, SaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options. |

### save(String filename, int format) {#save-java.lang.String-int-}
```
public final void save(String filename, int format)
```


Saves the project data to the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| format | int | The save file format. |

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(OutputStream stream, SaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SaveOptions-}
```
public final void save(OutputStream stream, SaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options. |

### save(OutputStream stream, MPPSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.MPPSaveOptions-}
```
public void save(OutputStream stream, MPPSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [MPPSaveOptions](../../com.aspose.tasks/mppsaveoptions) | The save options. |

### save(OutputStream stream, int format) {#save-java.io.OutputStream-int-}
```
public void save(OutputStream stream, int format)
```


Saves the project data to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| format | int | the specified save file format.[SaveFileFormat](../../com.aspose.tasks/savefileformat) |

### saveAsTemplate(String fileName, SaveTemplateOptions options) {#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-}
```
public void saveAsTemplate(String fileName, SaveTemplateOptions options)
```


Saves the project as a template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

### saveAsTemplate(OutputStream stream) {#saveAsTemplate-java.io.OutputStream-}
```
public final void saveAsTemplate(OutputStream stream)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save the project to. |

### saveAsTemplate(OutputStream stream, SaveTemplateOptions options) {#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-}
```
public final void saveAsTemplate(OutputStream stream, SaveTemplateOptions options)
```


Saves the project as a template to a specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | Stream to save the project template to. |
| options | [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions) | the specified save options [SaveTemplateOptions](../../com.aspose.tasks/savetemplateoptions). |

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

### saveReport(OutputStream stream, int reportType) {#saveReport-java.io.OutputStream-int-}
```
public void saveReport(OutputStream stream, int reportType)
```


Saves the project report of the specified type to the specified stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | the specified stream to save project report to. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### saveReport(String fileName, int reportType) {#saveReport-java.lang.String-int-}
```
public final void saveReport(String fileName, int reportType)
```


Saves the project report of the specified type in PDF format to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |
| reportType | int | the specified report type.[ReportType](../../com.aspose.tasks/reporttype) |

### selectAllChildTasks() {#selectAllChildTasks--}
```
public final List<Task> selectAllChildTasks()
```


Recursively collects all child tasks of the root task.

**Returns:**
java.util.List&lt;com.aspose.tasks.Task&gt; - The collection of tasks.
### &lt;T&gt;set(Key&lt;T,Integer&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Integer--T-}
```
public final void <T>set(Key<T,Integer> key, T val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Integer&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | T | the value.

 T : the type of the mapped value. |

### set(Key&lt;Date,Integer&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Integer--java.util.Date-}
```
public final void set(Key<Date,Integer> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Integer&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setBaseline(int baselineType) {#setBaseline-int-}
```
public final void setBaseline(int baselineType)
```


Saves baseline fields to the specified baseline for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |

### setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection) {#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--}
```
public final void setBaseline(int baselineType, Iterable<Task> taskCollection)
```


Saves baseline fields to the specified baseline for the selected tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineType | int | The baseline type to save baseline data to. |
| taskCollection | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | List of tasks to save baseline data for. |

### setBaselineSaveTime(int baselineNumber, Date value) {#setBaselineSaveTime-int-java.util.Date-}
```
public final void setBaselineSaveTime(int baselineNumber, Date value)
```


Sets the baseline save time.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baselineNumber | int | The baseline's number [BaselineType](../../com.aspose.tasks/baselinetype). |
| value | java.util.Date | The baseline's last save date and time.

--------------------

Set value to DateTime.MinValue if the baseline was not saved. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly) {#updateProjectWorkAsComplete-java.util.Date-boolean-}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)
```


Updates all work as complete through a specified date for the entire project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |

### updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection) {#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--}
```
public final void updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```


Updates all work as complete through a specified date for the specified list of tasks.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| completeThrough | java.util.Date | The date to update work as completed through. |
| setZeroOrHundredPercentCompleteOnly | boolean | If set to true updates only those tasks as 100% complete whose finish date is before specified complete-through date. Otherwise, calculates a percentage complete value based on scheduled start and complete-through dates. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to update work for. |

