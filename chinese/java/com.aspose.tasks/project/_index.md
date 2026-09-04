---
title: "项目"
second_title: "Aspose.Tasks for Java API 参考"
description: "表示一个项目。"
type: docs
weight: 220
url: /zh/java/com.aspose.tasks/project/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.IContainer
```
public class Project extends IContainer<Byte>
```

表示一个项目。

--------------------

该 **Project** 是 Aspose.Tasks 库中的核心类。

可以使用 **Project** 读取受支持的项目管理格式之一：MPP、MPT、MPX、XML。

要在任意受支持的格式中加载现有文档，请将文件名或流传递给 **Project** 的构造函数之一。要创建空项目，请调用无参数构造函数。

使用 Save 方法的任意重载，将项目保存为 [SaveFileFormat](../../com.aspose.tasks/savefileformat) 支持的任意格式：Primavera：P6 XML、PM XER；Microsoft Excel：XLSX、XML；固定布局：PDF；图像：JPEG、PNG、BMP、TIFF、SVG；文本：TXT；其他：HTML。

要打印项目，请使用 [print()](../../com.aspose.tasks/project\#print--) 方法的任意重载。

**Project** 存储项目范围的信息，例如 `Aspose.Tasks.Project.Views`([getViews()](../../com.aspose.tasks/project\#getViews--)/[setViews(ViewCollection)](../../com.aspose.tasks/project\#setViews-ViewCollection-))、`Aspose.Tasks.Project.BuiltInProps`([getBuiltInProps()](../../com.aspose.tasks/project\#getBuiltInProps--)/[setBuiltInProps(BuiltInProjectPropertyCollection)](../../com.aspose.tasks/project\#setBuiltInProps-BuiltInProjectPropertyCollection-))、`Aspose.Tasks.Project.CustomProps`([getCustomProps()](../../com.aspose.tasks/project\#getCustomProps--)/[setCustomProps(CustomProjectPropertyCollection)](../../com.aspose.tasks/project\#setCustomProps-CustomProjectPropertyCollection-)) 和 `Aspose.Tasks.Project.ExtendedAttributes`([getExtendedAttributes()](../../com.aspose.tasks/project\#getExtendedAttributes--)/[setExtendedAttributes(ExtendedAttributeDefinitionCollection)](../../com.aspose.tasks/project\#setExtendedAttributes-ExtendedAttributeDefinitionCollection-))。这些对象大多数可通过 **Project** 类的相应属性访问。

**Project** 是根实体，包含用于操作其他项目实体的入口点，例如 [Task](../../com.aspose.tasks/task)、[Resource](../../com.aspose.tasks/resource)、[ResourceAssignment](../../com.aspose.tasks/resourceassignment)、[ExtendedAttribute](../../com.aspose.tasks/extendedattribute) 和 [Calendar](../../com.aspose.tasks/calendar)。

**Project** 实体可通过类型化集合访问，例如 `Aspose.Tasks.Task.Children`([Task.getChildren()](../../com.aspose.tasks/task\#getChildren--)/[Task.setChildren(TaskCollection)](../../com.aspose.tasks/task\#setChildren-TaskCollection-))、`Aspose.Tasks.Project.Resources`([getResources()](../../com.aspose.tasks/project\#getResources--)/[setResources(ResourceCollection)](../../com.aspose.tasks/project\#setResources-ResourceCollection-))、`Aspose.Tasks.Project.ResourceAssignments`([getResourceAssignments()](../../com.aspose.tasks/project\#getResourceAssignments--)/[setResourceAssignments(ResourceAssignmentCollection)](../../com.aspose.tasks/project\#setResourceAssignments-ResourceAssignmentCollection-))，等等。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [Project()](#Project--) | 初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(String projectTemplate, String protectionPassword)](#Project-java.lang.String-java.lang.String-) | 从受密码保护的模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(String projectTemplate)](#Project-java.lang.String-) | 从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(InputStream stream, PrimaveraReadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-) | 使用指定的 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类实例，从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(String projectTemplate, ParseErrorCallback parseErrorHandler)](#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-) | 从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(InputStream stream)](#Project-java.io.InputStream-) | 从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(String projectTemplate, PrimaveraReadOptions options)](#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-) | 从模板（现有 MPP 或 MPT 文件）并使用指定的 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类实例，初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(DbSettings settings)](#Project-com.aspose.tasks.DbSettings-) | 初始化 [Project](../../com.aspose.tasks/project) 类的新实例，以读取由 [DbSettings](../../com.aspose.tasks/dbsettings) 类实例指定的数据库中的数据。 |
| [Project(InputStream stream, ParseErrorCallback parseErrorHandler)](#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-) | 从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(InputStream stream, String protectionPassword)](#Project-java.io.InputStream-java.lang.String-) | 从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(String projectTemplate, LoadOptions options)](#Project-java.lang.String-com.aspose.tasks.LoadOptions-) | 从模板（现有 mpp 或 mpt 文件）并使用指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例，初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
| [Project(InputStream stream, LoadOptions options)](#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-) | 使用指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例，从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [&lt;T&gt;get(Key&lt;T,Byte&gt; key)](#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--) | 返回此容器中属性映射的值。 |
| [&lt;T&gt;set(Key&lt;T,Byte&gt; key, T val)](#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-) | 将指定属性映射到此容器中的指定值。 |
| [copyTo(Project another)](#copyTo-com.aspose.tasks.Project-) | 将项目的主要数据和属性复制到另一个项目。 |
| [copyTo(Project another, CopyToOptions options)](#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-) | 将项目的主要数据和属性复制到另一个项目。 |
| [enumerateAllChildTasks()](#enumerateAllChildTasks--) | 递归枚举项目的所有任务，包括根任务。 |
| [getActualsInSync()](#getActualsInSync--) | 获取一个值，指示 ActualsInSync 是否已设置。 |
| [getAdminProject()](#getAdminProject--) | 获取一个值，指示 AdminProject 是否已设置。 |
| [getAreEditableActualCosts()](#getAreEditableActualCosts--) | 获取一个值，指示 AreEditableActualCosts 是否已设置。 |
| [getAuthor()](#getAuthor--) | 获取 Author 的值。 |
| [getAutoAddNewResourcesAndTasks()](#getAutoAddNewResourcesAndTasks--) | 获取一个值，指示是否已设置 AutoAddNewResourcesAndTasks。 |
| [getAutoCalculateAssignmentCosts()](#getAutoCalculateAssignmentCosts--) | 获取是否应使用分配的工作和资源费率自动计算分配成本和剩余成本。 |
| [getAutolink()](#getAutolink--) | 获取一个值，指示是否已设置 Autolink。 |
| [getBaselineForEarnedValue()](#getBaselineForEarnedValue--) | 获取 BaselineForEarnedValue 的值。 |
| [getBaselineSaveTime(int baselineNumber)](#getBaselineSaveTime-int-) | 返回基线保存时间。 |
| [getBuiltInProps()](#getBuiltInProps--) | 获取项目的内置属性集合。 |
| [getCalculationMode()](#getCalculationMode--) | 获取项目的计算模式。 |
| [getCalendar()](#getCalendar--) | 获取 Calendar 的值。 |
| [getCalendars()](#getCalendars--) | 获取此 Project 实例的 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 对象。 |
| [getCategory()](#getCategory--) | 获取 Category 的值。 |
| [getComments()](#getComments--) | 获取 Comments 的值。 |
| [getCompany()](#getCompany--) | 获取 Company 的值。 |
| [getCreationDate()](#getCreationDate--) | 获取 CreationDate 的值。 |
| [getCriticalPath()](#getCriticalPath--) | 获取一个集合，其中包含构成此项目关键路径的关键任务列表。 |
| [getCriticalSlackLimit()](#getCriticalSlackLimit--) | 如果总浮动小于或等于此天数，MS Project 将任务视为关键。 |
| [getCurrencyCode()](#getCurrencyCode--) | 获取 CurrencyCode 的值。 |
| [getCurrencyDigits()](#getCurrencyDigits--) | 获取 CurrencyDigits 的值。 |
| [getCurrencySymbol()](#getCurrencySymbol--) | 获取 CurrencySymbol 的值。 |
| [getCurrencySymbolPosition()](#getCurrencySymbolPosition--) | 获取 CurrencySymbolPosition 的值。 |
| [getCurrentDate()](#getCurrentDate--) | 获取 CurrentDate 的值。 |
| [getCustomDateFormat()](#getCustomDateFormat--) | 获取 CustomDateFormat 的值。 |
| [getCustomProps()](#getCustomProps--) | 获取项目的自定义属性集合。 |
| [getDateFormat()](#getDateFormat--) | 获取 DateFormat 的值。 |
| [getDaysPerMonth()](#getDaysPerMonth--) | 获取 DaysPerMonth 的值。 |
| [getDefaultFinishTime()](#getDefaultFinishTime--) | 获取 DefaultFinishTime 的值。 |
| [getDefaultFixedCostAccrual()](#getDefaultFixedCostAccrual--) | 获取 DefaultFixedCostAccrual 的值。 |
| [getDefaultOvertimeRate()](#getDefaultOvertimeRate--) | 获取 DefaultOvertimeRate 的值。 |
| [getDefaultStandardRate()](#getDefaultStandardRate--) | 获取 DefaultStandardRate 的值。 |
| [getDefaultStartTime()](#getDefaultStartTime--) | 获取 DefaultStartTime 的值。 |
| [getDefaultTaskEVMethod()](#getDefaultTaskEVMethod--) | 获取 DefaultTaskEVMethod 的值。 |
| [getDefaultTaskType()](#getDefaultTaskType--) | 获取 DefaultTaskType 的值。 |
| [getDefaultView()](#getDefaultView--) | 获取项目的默认视图。 |
| [getDefaultWeekWorkingDays()](#getDefaultWeekWorkingDays--) | 获取 [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 类的实例，该类表示项目默认工作周的工作日和工作时间的集合。 |
| [getDisplayOptions()](#getDisplayOptions--) | 获取 [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) 类的实例。 |
| [getDuration(double val)](#getDuration-double-) | 获取具有指定单位数量和默认持续时间格式的 [Duration](../../com.aspose.tasks/duration) 对象，默认格式在项目设置 [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) 中定义。 |
| [getDuration(double val, byte timeUnit)](#getDuration-double-byte-) | 获取具有指定数量的 [TimeUnitType](../../com.aspose.tasks/timeunittype) 单位的 [Duration](../../com.aspose.tasks/duration) 对象。 |
| [getDurationFormat()](#getDurationFormat--) | 获取 DurationFormat 的值。 |
| [getEarnedValueMethod()](#getEarnedValueMethod--) | 获取 EarnedValueMethod 的值。 |
| [getExtendedAttributes()](#getExtendedAttributes--) | 获取 ExtendedAttributeDefinitionCollection 对象。 |
| [getExtendedCreationDate()](#getExtendedCreationDate--) | 获取 ExtendedCreationDate 的值。 |
| [getFinishDate()](#getFinishDate--) | 获取 FinishDate 的值。 |
| [getFiscalYearStart()](#getFiscalYearStart--) | 获取一个值，指示是否已设置 FiscalYearStart。 |
| [getFyStartDate()](#getFyStartDate--) | 获取 FyStartDate 的值。 |
| [getGlobalizationSettings()](#getGlobalizationSettings--) | 获取项目的全球化（特定语言）设置。 |
| [getGuid()](#getGuid--) | 获取 Guid 的值。 |
| [getHonorConstraints()](#getHonorConstraints--) | 获取一个值，指示是否已设置 HonorConstraints。 |
| [getHyperlinkBase()](#getHyperlinkBase--) | 获取 HyperlinkBase 的值。 |
| [getInsertedProjectsLikeSummary()](#getInsertedProjectsLikeSummary--) | 获取一个值，指示是否已设置 InsertedProjectsLikeSummary。 |
| [getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()](#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--) | 获取一个值，指示是否已设置 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled。 |
| [getKeywords()](#getKeywords--) | 获取 Keywords 的值。 |
| [getLastAuthor()](#getLastAuthor--) | 获取 LastAuthor 的值。 |
| [getLastPrinted()](#getLastPrinted--) | 获取 LastPrinted 的值。 |
| [getLastSaved()](#getLastSaved--) | 获取 LastSaved 的值。 |
| [getManager()](#getManager--) | 获取 Manager 的值。 |
| [getMicrosoftProjectServerURL()](#getMicrosoftProjectServerURL--) | 获取一个值，指示 MicrosoftProjectServerURL 是否已设置。 |
| [getMinutesPerDay()](#getMinutesPerDay--) | 获取 MinutesPerDay 的值。 |
| [getMinutesPerWeek()](#getMinutesPerWeek--) | 获取 MinutesPerWeek 的值。 |
| [getMoveCompletedEndsBack()](#getMoveCompletedEndsBack--) | 获取一个值，指示 MoveCompletedEndsBack 是否已设置。 |
| [getMoveCompletedEndsForward()](#getMoveCompletedEndsForward--) | 获取一个值，指示 MoveCompletedEndsForward 是否已设置。 |
| [getMoveRemainingStartsBack()](#getMoveRemainingStartsBack--) | 获取一个值，指示 MoveRemainingStartsBack 是否已设置。 |
| [getMoveRemainingStartsForward()](#getMoveRemainingStartsForward--) | 获取一个值，指示 MoveRemainingStartsForward 是否已设置。 |
| [getMultipleCriticalPaths()](#getMultipleCriticalPaths--) | 获取一个值，指示 MultipleCriticalPaths 是否已设置。 |
| [getName()](#getName--) | 获取 Name 的值。 |
| [getNewTaskStartDate()](#getNewTaskStartDate--) | 获取 NewTaskStartDate 的值。 |
| [getNewTasksAreManual()](#getNewTasksAreManual--) | 获取一个值，指示 NewTasksAreManual 是否已设置。 |
| [getNewTasksEffortDriven()](#getNewTasksEffortDriven--) | 获取一个值，指示 NewTasksEffortDriven 是否已设置。 |
| [getNewTasksEstimated()](#getNewTasksEstimated--) | 获取一个值，指示 NewTasksEstimated 是否已设置。 |
| [getOleObjects()](#getOleObjects--) | 获取一个集合，包含链接或嵌入到此项目文件的 [OleObject](../../com.aspose/tasks/oleobject) 类实例。 |
| [getOutlineCodes()](#getOutlineCodes--) | 获取 OutlineCodeDefinitionCollection 对象。 |
| [getPageCount()](#getPageCount--) | 返回使用默认 [Timescale](../../com.aspose.tasks/timescale)（天）渲染项目的页数。 |
| [getPageCount(SaveOptions saveOptions)](#getPageCount-com.aspose.tasks.SaveOptions-) | 返回使用给定的 [SaveOptions](../../com.aspose.tasks/saveoptions) 渲染项目的页数。 |
| [getPageCount(int format, int scale)](#getPageCount-int-int-) | 返回使用给定的 [Timescale](../../com.aspose.tasks/timescale) 和 [PresentationFormat](../../com.aspose.tasks/presentationformat) 渲染项目的页数。 |
| [getPageCount_PageSize(int pageSize, int scale)](#getPageCount-PageSize-int-int-) | 返回使用给定的 [Timescale](../../com.aspose.tasks/timescale) 和 [PageSize](../../com.aspose.tasks/pagesize) 渲染项目的页数。 |
| [getPageCount_PageSize(int pageSize, int scale, Date startDate, Date endDate)](#getPageCount-PageSize-int-int-java.util.Date-java.util.Date-) | 返回使用给定的 [Timescale](../../com.aspose.tasks/timescale)、[PresentationFormat](../../com.aspose.tasks/presentationformat) 和日期范围渲染项目的页数。 |
| [getPageCount_PresentationFormat(int format)](#getPageCount-PresentationFormat-int-) | 返回使用默认 [Timescale](../../com.aspose.tasks/timescale)（天）和给定的 [PresentationFormat](../../com.aspose.tasks/presentationformat) 渲染项目的页数。 |
| [getPageCount_Timescale(int scale)](#getPageCount-Timescale-int-) | 返回使用给定的 [Timescale](../../com.aspose.tasks/timescale) 渲染项目的页数。 |
| [getPredecessors(Task task)](#getPredecessors-com.aspose.tasks.Task-) | 返回指定任务的前置任务链接集合。 |
| [getPrimaveraProperties()](#getPrimaveraProperties--) | 获取一个包含从 Primavera 文件读取的项目的 Primavera 特定属性的对象。 |
| [getProjectExternallyEdited()](#getProjectExternallyEdited--) | 获取一个指示是否已设置 ProjectExternallyEdited 的值。 |
| [getProjectFileInfo(InputStream stream)](#getProjectFileInfo-java.io.InputStream-) | 从流中获取项目文件信息。 |
| [getProjectFileInfo(String filename)](#getProjectFileInfo-java.lang.String-) | 从文件读取项目文件信息。 |
| [getRemoveFileProperties()](#getRemoveFileProperties--) | 获取一个指示是否已设置 RemoveFileProperties 的值。 |
| [getResourceAssignments()](#getResourceAssignments--) | 获取 ResourceAssignmentCollection 对象。 |
| [getResourceFilters()](#getResourceFilters--) | 获取所有基于资源的过滤器定义。 |
| [getResourceGroups()](#getResourceGroups--) | 获取所有基于资源的组定义。 |
| [getResources()](#getResources--) | 获取 ResourceCollection 对象。 |
| [getRevision()](#getRevision--) | 获取 Revision 的值。 |
| [getRootTask()](#getRootTask--) | 获取任务树的根节点。 |
| [getSaveVersion()](#getSaveVersion--) | 获取 SaveVersion 的值。 |
| [getScheduleFromStart()](#getScheduleFromStart--) | 获取一个指示是否已设置 ScheduleFromStart 的值。 |
| [getShowProjectSummaryTask()](#getShowProjectSummaryTask--) | 获取一个指示是否已设置 ShowProjectSummaryTask 的值。 |
| [getSplitsInProgressTasks()](#getSplitsInProgressTasks--) | 获取一个指示是否已设置 SplitsInProgressTasks 的值。 |
| [getSpreadActualCost()](#getSpreadActualCost--) | 获取一个指示是否已设置 SpreadActualCost 的值。 |
| [getSpreadPercentComplete()](#getSpreadPercentComplete--) | 获取一个指示是否已设置 SpreadPercentComplete 的值。 |
| [getStartDate()](#getStartDate--) | 获取 StartDate 的值。 |
| [getStatusDate()](#getStatusDate--) | 获取 StatusDate 的值。 |
| [getSubject()](#getSubject--) | 获取 Subject 的值。 |
| [getTables()](#getTables--) | 获取一个 [Table](../../com.aspose.tasks/table) 对象列表。 |
| [getTaskFilters()](#getTaskFilters--) | 获取所有基于任务的过滤器定义。 |
| [getTaskGroups()](#getTaskGroups--) | 获取所有基于任务的组定义。 |
| [getTaskLinks()](#getTaskLinks--) | 获取 [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) 对象。 |
| [getTaskUpdatesResource()](#getTaskUpdatesResource--) | 获取一个指示是否已设置 TaskUpdatesResource 的值。 |
| [getTemplate()](#getTemplate--) | 获取 Template 的值。 |
| [getTimescaleFinish()](#getTimescaleFinish--) | 获取 TimescaleFinish 的值。 |
| [getTimescaleStart()](#getTimescaleStart--) | 获取 TimescaleStart 的值。 |
| [getTitle()](#getTitle--) | 获取 Title 的值。 |
| [getUid()](#getUid--) | 获取 Uid 的值。 |
| [getUpdateManuallyScheduledTasksWhenEditingLinks()](#getUpdateManuallyScheduledTasksWhenEditingLinks--) | 获取一个值，指示 UpdateManuallyScheduledTasksWhenEditingLinks 是否已设置。 |
| [getVbaProject()](#getVbaProject--) | 获取 `VbaProject` 类的实例（[getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-))。 |
| [getViews()](#getViews--) | 获取 [View](../../com.aspose.tasks/view) 对象的列表。 |
| [getWBSCodeDefinition()](#getWBSCodeDefinition--) | 获取项目的 WBS Code Definition。 |
| [getWeekStartDay()](#getWeekStartDay--) | 获取 WeekStartDay 的值。 |
| [getWork(double val)](#getWork-double-) | 获取具有指定 `double` 值和默认工作格式的 [Duration](../../com.aspose.tasks/duration) 对象。 |
| [getWorkFormat()](#getWorkFormat--) | 获取 WorkFormat 的值。 |
| [print()](#print--) | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机并使用默认打印机设置。 |
| [print(PrintOptions options)](#print-com.aspose.tasks.PrintOptions-) | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置和自定义保存选项。 |
| [print(PrinterSettings printerSettings)](#print-com.aspose.tasks.PrinterSettings-) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| [print(PrinterSettings printerSettings, PrintOptions options)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置和自定义保存选项打印项目。 |
| [print(PrinterSettings printerSettings, PrintOptions options, String documentName)](#print-com.aspose.tasks.PrinterSettings-com.aspose.tasks.PrintOptions-java.lang.String-) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置、自定义保存选项和指定的文档名称打印项目。 |
| [print(PrinterSettings printerSettings, String documentName)](#print-com.aspose.tasks.PrinterSettings-java.lang.String-) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| [print(String printerName)](#print-java.lang.String-) | 使用标准（无用户界面）打印控制器，将项目打印到指定的打印机并使用默认打印机设置。 |
| [recalculate()](#recalculate--) | 重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算余量、工作和成本字段。 |
| [recalculate(boolean validate)](#recalculate-boolean-) | 重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算余量、工作和成本字段，可选进行验证。 |
| [recalculateResourceFields()](#recalculateResourceFields--) | 重新计算资源的 ID、开始和结束。 |
| [recalculateResourceStartFinish()](#recalculateResourceStartFinish--) | 重新计算资源的开始和结束。 |
| [removeInvalidResourceAssignments()](#removeInvalidResourceAssignments--) | 从项目资源分配列表中消除无效的资源分配。 |
| [renumberWBSCode()](#renumberWBSCode--) | 重新编号所有任务的 WBS 代码。 |
| [renumberWBSCode(List&lt;Integer&gt; taskIds)](#renumberWBSCode-java.util.List-java.lang.Integer--) | 重新编号已传递任务的 WBS 代码。 |
| [rescheduleUncompletedWorkToStartAfter(Date after)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-) | 重新安排未完成的项目工作，使其在指定日期之后开始。 |
| [rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection)](#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--) | 将指定任务列表中未完成的工作重新安排，以在指定日期之后开始。 |
| [save(OutputStream stream, SimpleSaveOptions options)](#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-) | 使用指定的保存选项将项目保存到流中。 |
| [save(OutputStream stream, int format)](#save-java.io.OutputStream-int-) | 将项目数据保存到流中。 |
| [save(String filename)](#save-java.lang.String-) | 以 mpp 格式将项目数据保存到文件中。 |
| [save(String filename, SimpleSaveOptions options)](#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-) | 使用指定的保存选项将文档保存到文件中。 |
| [save(String filename, int format)](#save-java.lang.String-int-) | 将项目数据保存到文件中。 |
| [saveAsTemplate(OutputStream stream)](#saveAsTemplate-java.io.OutputStream-) | 将项目作为模板保存到指定的流中。 |
| [saveAsTemplate(OutputStream stream, SaveTemplateOptions options)](#saveAsTemplate-java.io.OutputStream-com.aspose.tasks.SaveTemplateOptions-) | 将项目作为模板保存到指定的流中。 |
| [saveAsTemplate(String fileName)](#saveAsTemplate-java.lang.String-) | 将项目作为模板保存到指定的文件路径。 |
| [saveAsTemplate(String fileName, SaveTemplateOptions options)](#saveAsTemplate-java.lang.String-com.aspose.tasks.SaveTemplateOptions-) | 将项目保存为模板。 |
| [saveReport(OutputStream stream)](#saveReport-java.io.OutputStream-) | 将项目概览报告保存到流中。 |
| [saveReport(OutputStream stream, int reportType)](#saveReport-java.io.OutputStream-int-) | 将指定类型的项目报告保存到指定的流中。 |
| [saveReport(String fileName)](#saveReport-java.lang.String-) | 将项目概览报告保存为 PDF 文件。 |
| [saveReport(String fileName, int reportType)](#saveReport-java.lang.String-int-) | 将指定类型的项目报告以 PDF 格式保存到指定的文件路径。 |
| [selectAllChildTasks()](#selectAllChildTasks--) | 递归收集根任务的所有子任务。 |
| [set(Key&lt;Date,Byte&gt; key, Date val)](#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-) | 将指定属性映射到此容器中的指定值。 |
| [setActualsInSync(NullableBool value)](#setActualsInSync-com.aspose.tasks.NullableBool-) | 设置一个值，指示 ActualsInSync 是否已设置。 |
| [setAdminProject(NullableBool value)](#setAdminProject-com.aspose.tasks.NullableBool-) | 设置一个值，指示 AdminProject 是否已设置。 |
| [setAreEditableActualCosts(NullableBool value)](#setAreEditableActualCosts-com.aspose.tasks.NullableBool-) | 设置一个值，指示 AreEditableActualCosts 是否已设置。 |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | 设置 Author 的值。 |
| [setAutoAddNewResourcesAndTasks(NullableBool value)](#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-) | 设置一个值，指示 AutoAddNewResourcesAndTasks 是否已设置。 |
| [setAutoCalculateAssignmentCosts(boolean value)](#setAutoCalculateAssignmentCosts-boolean-) | 设置是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| [setAutolink(NullableBool value)](#setAutolink-com.aspose.tasks.NullableBool-) | 设置一个值，指示 Autolink 是否已设置。 |
| [setBaseline(int baselineType)](#setBaseline-int-) | 将基线字段保存到整个项目的指定基线。 |
| [setBaseline(int baselineType, Iterable&lt;Task&gt; taskCollection)](#setBaseline-int-java.lang.Iterable-com.aspose.tasks.Task--) | 将基线字段保存到所选任务的指定基线。 |
| [setBaselineForEarnedValue(int value)](#setBaselineForEarnedValue-int-) | 设置 BaselineForEarnedValue 的值。 |
| [setBaselineSaveTime(int baselineNumber, Date value)](#setBaselineSaveTime-int-java.util.Date-) | 设置基线保存时间。 |
| [setCalculationMode(int value)](#setCalculationMode-int-) | 设置 项目 的计算模式。 |
| [setCalendar(Calendar value)](#setCalendar-com.aspose.tasks.Calendar-) | 设置 Calendar 的值。 |
| [setCategory(String value)](#setCategory-java.lang.String-) | 设置 Category 的值。 |
| [setComments(String value)](#setComments-java.lang.String-) | 设置 Comments 的值。 |
| [setCompany(String value)](#setCompany-java.lang.String-) | 设置 Company 的值。 |
| [setCreationDate(Date value)](#setCreationDate-java.util.Date-) | 设置 CreationDate 的值。 |
| [setCriticalSlackLimit(int value)](#setCriticalSlackLimit-int-) | 如果总浮动小于或等于此天数，MS Project 将任务视为关键。 |
| [setCurrencyCode(String value)](#setCurrencyCode-java.lang.String-) | 设置 CurrencyCode 的值。 |
| [setCurrencyDigits(int value)](#setCurrencyDigits-int-) | 设置 CurrencyDigits 的值。 |
| [setCurrencySymbol(String value)](#setCurrencySymbol-java.lang.String-) | 设置 CurrencySymbol 的值。 |
| [setCurrencySymbolPosition(int value)](#setCurrencySymbolPosition-int-) | 设置 CurrencySymbolPosition 的值。 |
| [setCurrentDate(Date value)](#setCurrentDate-java.util.Date-) | 设置 CurrentDate 的值。 |
| [setCustomDateFormat(String value)](#setCustomDateFormat-java.lang.String-) | 设置 CustomDateFormat 的值。 |
| [setDateFormat(int value)](#setDateFormat-int-) | 设置 DateFormat 的值。 |
| [setDaysPerMonth(int value)](#setDaysPerMonth-int-) | 设置 DaysPerMonth 的值。 |
| [setDefaultFinishTime(Date value)](#setDefaultFinishTime-java.util.Date-) | 设置 DefaultFinishTime 的值。 |
| [setDefaultFixedCostAccrual(int value)](#setDefaultFixedCostAccrual-int-) | 设置 DefaultFixedCostAccrual 的值。 |
| [setDefaultOvertimeRate(double value)](#setDefaultOvertimeRate-double-) | 设置 DefaultOvertimeRate 的值。 |
| [setDefaultStandardRate(double value)](#setDefaultStandardRate-double-) | 设置 DefaultStandardRate 的值。 |
| [setDefaultStartTime(Date value)](#setDefaultStartTime-java.util.Date-) | 设置 DefaultStartTime 的值。 |
| [setDefaultTaskEVMethod(int value)](#setDefaultTaskEVMethod-int-) | 设置 DefaultTaskEVMethod 的值。 |
| [setDefaultTaskType(int value)](#setDefaultTaskType-int-) | 设置 DefaultTaskType 的值。 |
| [setDefaultView(View value)](#setDefaultView-com.aspose.tasks.View-) | 设置 项目 的默认视图。 |
| [setDurationFormat(byte value)](#setDurationFormat-byte-) | 设置 DurationFormat 的值。 |
| [setEarnedValueMethod(int value)](#setEarnedValueMethod-int-) | 设置 EarnedValueMethod 的值。 |
| [setExtendedCreationDate(Date value)](#setExtendedCreationDate-java.util.Date-) | 设置 ExtendedCreationDate 的值。 |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | 设置 FinishDate 的值。 |
| [setFiscalYearStart(NullableBool value)](#setFiscalYearStart-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 FiscalYearStart。 |
| [setFyStartDate(int value)](#setFyStartDate-int-) | 设置 FyStartDate 的值。 |
| [setGlobalizationSettings(GlobalizationSettings value)](#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-) | 设置项目的全球化（语言特定）设置。 |
| [setGuid(UUID value)](#setGuid-java.util.UUID-) | 设置 Guid 的值。 |
| [setHonorConstraints(NullableBool value)](#setHonorConstraints-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 HonorConstraints。 |
| [setHyperlinkBase(String value)](#setHyperlinkBase-java.lang.String-) | 设置 HyperlinkBase 的值。 |
| [setInsertedProjectsLikeSummary(NullableBool value)](#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 InsertedProjectsLikeSummary。 |
| [setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)](#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled。 |
| [setKeywords(String value)](#setKeywords-java.lang.String-) | 设置 Keywords 的值。 |
| [setLastAuthor(String value)](#setLastAuthor-java.lang.String-) | 设置 LastAuthor 的值。 |
| [setLastPrinted(Date value)](#setLastPrinted-java.util.Date-) | 设置 LastPrinted 的值。 |
| [setLastSaved(Date value)](#setLastSaved-java.util.Date-) | 设置 LastSaved 的值。 |
| [setManager(String value)](#setManager-java.lang.String-) | 设置 Manager 的值。 |
| [setMicrosoftProjectServerURL(NullableBool value)](#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MicrosoftProjectServerURL。 |
| [setMinutesPerDay(int value)](#setMinutesPerDay-int-) | 设置 MinutesPerDay 的值。 |
| [setMinutesPerWeek(int value)](#setMinutesPerWeek-int-) | 设置 MinutesPerWeek 的值。 |
| [setMoveCompletedEndsBack(NullableBool value)](#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MoveCompletedEndsBack。 |
| [setMoveCompletedEndsForward(NullableBool value)](#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MoveCompletedEndsForward。 |
| [setMoveRemainingStartsBack(NullableBool value)](#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MoveRemainingStartsBack。 |
| [setMoveRemainingStartsForward(NullableBool value)](#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MoveRemainingStartsForward。 |
| [setMultipleCriticalPaths(NullableBool value)](#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 MultipleCriticalPaths。 |
| [setName(String value)](#setName-java.lang.String-) | 设置 Name 的值。 |
| [setNewTaskStartDate(int value)](#setNewTaskStartDate-int-) | 设置 NewTaskStartDate 的值。 |
| [setNewTasksAreManual(NullableBool value)](#setNewTasksAreManual-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 NewTasksAreManual。 |
| [setNewTasksEffortDriven(NullableBool value)](#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 NewTasksEffortDriven。 |
| [setNewTasksEstimated(NullableBool value)](#setNewTasksEstimated-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 NewTasksEstimated。 |
| [setProjectExternallyEdited(NullableBool value)](#setProjectExternallyEdited-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 ProjectExternallyEdited。 |
| [setRemoveFileProperties(NullableBool value)](#setRemoveFileProperties-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 RemoveFileProperties。 |
| [setRevision(int value)](#setRevision-int-) | 设置 Revision 的值。 |
| [setSaveVersion(int value)](#setSaveVersion-int-) | 设置 SaveVersion 的值。 |
| [setScheduleFromStart(NullableBool value)](#setScheduleFromStart-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 ScheduleFromStart。 |
| [setShowProjectSummaryTask(boolean value)](#setShowProjectSummaryTask-boolean-) | 设置一个值，指示是否已设置 ShowProjectSummaryTask。 |
| [setSplitsInProgressTasks(NullableBool value)](#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 SplitsInProgressTasks。 |
| [setSpreadActualCost(NullableBool value)](#setSpreadActualCost-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 SpreadActualCost。 |
| [setSpreadPercentComplete(NullableBool value)](#setSpreadPercentComplete-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 SpreadPercentComplete。 |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | 设置 StartDate 的值。 |
| [setStatusDate(Date value)](#setStatusDate-java.util.Date-) | 设置 StatusDate 的值。 |
| [setSubject(String value)](#setSubject-java.lang.String-) | 设置 Subject 的值。 |
| [setTaskUpdatesResource(NullableBool value)](#setTaskUpdatesResource-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 TaskUpdatesResource。 |
| [setTemplate(String value)](#setTemplate-java.lang.String-) | 设置 Template 的值。 |
| [setTimescaleFinish(Date value)](#setTimescaleFinish-java.util.Date-) | 设置 TimescaleFinish 的值。 |
| [setTimescaleStart(Date value)](#setTimescaleStart-java.util.Date-) | 设置 TimescaleStart 的值。 |
| [setTitle(String value)](#setTitle-java.lang.String-) | 设置 Title 的值。 |
| [setUid(String value)](#setUid-java.lang.String-) | 设置 Uid 的值。 |
| [setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)](#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-) | 设置一个值，指示是否已设置 UpdateManuallyScheduledTasksWhenEditingLinks。 |
| [setWBSCodeDefinition(WBSCodeDefinition value)](#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-) | 为项目设置 WBS 代码定义。 |
| [setWeekStartDay(int value)](#setWeekStartDay-int-) | 设置 WeekStartDay 的值。 |
| [setWorkFormat(byte value)](#setWorkFormat-byte-) | 设置 WorkFormat 的值。 |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly)](#updateProjectWorkAsComplete-java.util.Date-boolean-) | 将整个项目的所有工作更新为截至指定日期的完成状态。 |
| [updateProjectWorkAsComplete(Date completeThrough, boolean setZeroOrHundredPercentCompleteOnly, List&lt;Task&gt; taskCollection)](#updateProjectWorkAsComplete-java.util.Date-boolean-java.util.List-com.aspose.tasks.Task--) | 将指定任务列表的所有工作更新为截至指定日期的完成状态。 |
### Project() {#Project--}
```
public Project()
```


初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

### Project(String projectTemplate, String protectionPassword) {#Project-java.lang.String-java.lang.String-}
```
public Project(String projectTemplate, String protectionPassword)
```


从受密码保护的模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 用于创建项目的模板路径。 |
|  | protectionPassword | java.lang.String | 保护密码。 |

--------------------

当前仅支持读取受密码保护的 MSP 2003 文件格式的文件。 |

### Project(String projectTemplate) {#Project-java.lang.String-}
```
public Project(String projectTemplate)
```


从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 用于创建项目的模板路径。 |

### Project(InputStream stream, PrimaveraReadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(InputStream stream, PrimaveraReadOptions options)
```


使用指定的 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类实例，从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 项目的流 java.io.InputStreamclass |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | 指定的 [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) 类实例，允许自定义读取 Primavera 格式（XER 或 XML）。 |

### Project(String projectTemplate, ParseErrorCallback parseErrorHandler) {#Project-java.lang.String-com.aspose.tasks.ParseErrorCallback-}
```
public Project(String projectTemplate, ParseErrorCallback parseErrorHandler)
```


从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 用于创建项目的模板路径。 |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | 指定的回调方法，用于处理 xml 解析错误。 |

### Project(InputStream stream) {#Project-java.io.InputStream-}
```
public Project(InputStream stream)
```


从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 用于加载模板的 java.io.InputStream。 |

### Project(String projectTemplate, PrimaveraReadOptions options) {#Project-java.lang.String-com.aspose.tasks.PrimaveraReadOptions-}
```
public Project(String projectTemplate, PrimaveraReadOptions options)
```


从模板（现有 MPP 或 MPT 文件）并使用指定的 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类实例，初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 用于创建项目的模板路径 |
| options | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | 指定的 [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) 类实例。 |

### Project(DbSettings settings) {#Project-com.aspose.tasks.DbSettings-}
```
public Project(DbSettings settings)
```


初始化 [Project](../../com.aspose.tasks/project) 类的新实例，以读取由 [DbSettings](../../com.aspose.tasks/dbsettings) 类实例指定的数据库中的数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| settings | [DbSettings](../../com.aspose.tasks/dbsettings) | 指定的 [DbSettings](../../com.aspose.tasks/dbsettings) 类实例。 |

### Project(InputStream stream, ParseErrorCallback parseErrorHandler) {#Project-java.io.InputStream-com.aspose.tasks.ParseErrorCallback-}
```
public Project(InputStream stream, ParseErrorCallback parseErrorHandler)
```


从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 用于加载模板的 java.io.InputStream。 |
| parseErrorHandler | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | 指定的回调方法，用于处理 xml 解析错误。 |

### Project(InputStream stream, String protectionPassword) {#Project-java.io.InputStream-java.lang.String-}
```
public Project(InputStream stream, String protectionPassword)
```


从模板（现有 mpp 或 mpt 文件）初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 用于加载模板的 java.io.InputStream。 |
|  | protectionPassword | java.lang.String | 保护密码。 |

--------------------

当前仅支持读取受密码保护的 MSP 2003 文件格式的文件。 |

### Project(String projectTemplate, LoadOptions options) {#Project-java.lang.String-com.aspose.tasks.LoadOptions-}
```
public Project(String projectTemplate, LoadOptions options)
```


从模板（现有 mpp 或 mpt 文件）并使用指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例，初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| projectTemplate | java.lang.String | 用于创建项目的模板路径 |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | 指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例。 |

### Project(InputStream stream, LoadOptions options) {#Project-java.io.InputStream-com.aspose.tasks.LoadOptions-}
```
public Project(InputStream stream, LoadOptions options)
```


使用指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例，从流中初始化 [Project](../../com.aspose.tasks/project) 类的新实例。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 流 | java.io.InputStream | 项目的流 java.io.InputStreamclass |
| options | [LoadOptions](../../com.aspose.tasks/loadoptions) | 指定的 [LoadOptions](../../com.aspose.tasks/loadoptions) 类实例 |

### &lt;T&gt;get(Key&lt;T,Byte&gt; key) {#-T-get-com.aspose.tasks.Key-T-java.lang.Byte--}
```
public final T <T>get(Key<T,Byte> key)
```


返回此容器中属性映射的值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。[Prj](../../com.aspose.tasks/prj) 用于获取属性键。 |

**Returns:**
T - 在此容器中映射到的属性值。
### &lt;T&gt;set(Key&lt;T,Byte&gt; key, T val) {#-T-set-com.aspose.tasks.Key-T-java.lang.Byte--T-}
```
public final void <T>set(Key<T,Byte> key, T val)
```


将指定属性映射到此容器中的指定值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;T,java.lang.Byte&gt; | 指定的属性键。[Prj](../../com.aspose.tasks/prj) 用于获取属性键。 |
| val | T | 该值。 |

### copyTo(Project another) {#copyTo-com.aspose.tasks.Project-}
```
public final void copyTo(Project another)
```


将项目的主要数据和属性复制到另一个项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | 另一个用于复制数据的项目。 |

### copyTo(Project another, CopyToOptions options) {#copyTo-com.aspose.tasks.Project-com.aspose.tasks.CopyToOptions-}
```
public final void copyTo(Project another, CopyToOptions options)
```


将项目的主要数据和属性复制到另一个项目。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| another | [Project](../../com.aspose.tasks/project) | 另一个用于复制数据的项目。 |
| options | [CopyToOptions](../../com.aspose.tasks/copytooptions) | 复制选项，用于控制复制过程。 |

### enumerateAllChildTasks() {#enumerateAllChildTasks--}
```
public final Iterable<Task> enumerateAllChildTasks()
```


递归枚举项目的所有任务，包括根任务。

**Returns:**
java.lang.Iterable&lt;com.aspose.tasks.Task&gt; - 可用于遍历所有项目任务的 IEnumerable。

--------------------

提供一种比 [selectAllChildTasks()](../../com.aspose.tasks/project\#selectAllChildTasks--) 方法更轻量的遍历任务方式，因为它不会为所有任务分配内存。
### getActualsInSync() {#getActualsInSync--}
```
public final NullableBool getActualsInSync()
```


获取一个值，指示 ActualsInSync 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ActualsInSync is set or not.
### getAdminProject() {#getAdminProject--}
```
public final NullableBool getAdminProject()
```


获取一个值，指示 AdminProject 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AdminProject is set or not.
### getAreEditableActualCosts() {#getAreEditableActualCosts--}
```
public final NullableBool getAreEditableActualCosts()
```


获取一个值，指示 AreEditableActualCosts 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AreEditableActualCosts is set or not.
### getAuthor() {#getAuthor--}
```
public final String getAuthor()
```


获取 Author 的值。

**Returns:**
java.lang.String - Author 的值。
### getAutoAddNewResourcesAndTasks() {#getAutoAddNewResourcesAndTasks--}
```
public final NullableBool getAutoAddNewResourcesAndTasks()
```


获取一个值，指示是否已设置 AutoAddNewResourcesAndTasks。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether AutoAddNewResourcesAndTasks is set or not.
### getAutoCalculateAssignmentCosts() {#getAutoCalculateAssignmentCosts--}
```
public final boolean getAutoCalculateAssignmentCosts()
```


获取是否应使用分配的工作和资源费率自动计算分配成本和剩余成本。

**Returns:**
boolean - 是否应使用分配的工作和资源费率自动计算分配成本和剩余成本。
### getAutolink() {#getAutolink--}
```
public final NullableBool getAutolink()
```


获取一个值，指示是否已设置 Autolink。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether Autolink is set or not.
### getBaselineForEarnedValue() {#getBaselineForEarnedValue--}
```
public final int getBaselineForEarnedValue()
```


获取 BaselineForEarnedValue 的值。

**Returns:**
int - BaselineForEarnedValue 的值。
### getBaselineSaveTime(int baselineNumber) {#getBaselineSaveTime-int-}
```
public final Date getBaselineSaveTime(int baselineNumber)
```


返回基线保存时间。如果基线未保存，则返回 DateTime.MinValue（00:00:00.0000000 UTC，公元 0001 年 1 月 1 日）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| baselineNumber | int | 基线的编号 [BaselineType](../../com.aspose.tasks/baselinetype)。 |

**Returns:**
java.util.Date - 基线的最近保存日期和时间。
### getBuiltInProps() {#getBuiltInProps--}
```
public final BuiltInProjectPropertyCollection getBuiltInProps()
```


获取项目的内置属性集合。

**Returns:**
[BuiltInProjectPropertyCollection](../../com.aspose.tasks/builtinprojectpropertycollection) - project's built-in properties collection.
### getCalculationMode() {#getCalculationMode--}
```
public final int getCalculationMode()
```


获取项目的计算模式。可以是 `CalculationMode` 枚举的其中一个值（[getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)）。

**Returns:**
int - 项目的计算模式。
### getCalendar() {#getCalendar--}
```
public final Calendar getCalendar()
```


获取 Calendar 的值。

**Returns:**
[Calendar](../../com.aspose.tasks/calendar) - a value of Calendar.
### getCalendars() {#getCalendars--}
```
public final CalendarCollection getCalendars()
```


获取此 Project 实例的 [CalendarCollection](../../com.aspose.tasks/calendarcollection) 对象。

**Returns:**
[CalendarCollection](../../com.aspose.tasks/calendarcollection) - [CalendarCollection](../../com.aspose.tasks/calendarcollection) object of this Project instance.
### getCategory() {#getCategory--}
```
public final String getCategory()
```


获取 Category 的值。

**Returns:**
java.lang.String - Category 的值。
### getComments() {#getComments--}
```
public final String getComments()
```


获取 Comments 的值。

**Returns:**
java.lang.String - Comments 的值。
### getCompany() {#getCompany--}
```
public final String getCompany()
```


获取 Company 的值。

**Returns:**
java.lang.String - Company 的值。
### getCreationDate() {#getCreationDate--}
```
public final Date getCreationDate()
```


获取 CreationDate 的值。

**Returns:**
java.util.Date - CreationDate 的值。
### getCriticalPath() {#getCriticalPath--}
```
public final TaskCollection getCriticalPath()
```


获取一个集合，其中包含构成此项目关键路径的关键任务列表。

**Returns:**
[TaskCollection](../../com.aspose.tasks/taskcollection) - a collection which represents a list of all critical tasks.

--------------------

这是一个 O(n) 操作，其中 n 是项目中任务的数量。
### getCriticalSlackLimit() {#getCriticalSlackLimit--}
```
public final int getCriticalSlackLimit()
```


如果总浮动小于或等于此天数，MS Project 将任务视为关键。

**Returns:**
int - 任务被视为关键的总浮动时间（以天为单位）的最大值
### getCurrencyCode() {#getCurrencyCode--}
```
public final String getCurrencyCode()
```


获取 CurrencyCode 的值。

**Returns:**
java.lang.String - CurrencyCode 的值。
### getCurrencyDigits() {#getCurrencyDigits--}
```
public final int getCurrencyDigits()
```


获取 CurrencyDigits 的值。

**Returns:**
int - CurrencyDigits 的值。
### getCurrencySymbol() {#getCurrencySymbol--}
```
public final String getCurrencySymbol()
```


获取 CurrencySymbol 的值。

**Returns:**
java.lang.String - CurrencySymbol 的值。
### getCurrencySymbolPosition() {#getCurrencySymbolPosition--}
```
public final int getCurrencySymbolPosition()
```


获取 CurrencySymbolPosition 的值。

**Returns:**
int - CurrencySymbolPosition 的值。
### getCurrentDate() {#getCurrentDate--}
```
public final Date getCurrentDate()
```


获取 CurrentDate 的值。

**Returns:**
java.util.Date - CurrentDate 的值。
### getCustomDateFormat() {#getCustomDateFormat--}
```
public final String getCustomDateFormat()
```


获取 CustomDateFormat 的值。

**Returns:**
java.lang.String - CustomDateFormat 的值。
### getCustomProps() {#getCustomProps--}
```
public final CustomProjectPropertyCollection getCustomProps()
```


获取项目的自定义属性集合。

**Returns:**
[CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection) - project's custom properties collection.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


获取 DateFormat 的值。

**Returns:**
int - DateFormat 的值。
### getDaysPerMonth() {#getDaysPerMonth--}
```
public final int getDaysPerMonth()
```


获取 DaysPerMonth 的值。

**Returns:**
int - DaysPerMonth 的值。
### getDefaultFinishTime() {#getDefaultFinishTime--}
```
public final Date getDefaultFinishTime()
```


获取 DefaultFinishTime 的值。

**Returns:**
java.util.Date - DefaultFinishTime 的值。
### getDefaultFixedCostAccrual() {#getDefaultFixedCostAccrual--}
```
public final int getDefaultFixedCostAccrual()
```


获取 DefaultFixedCostAccrual 的值。

**Returns:**
int - DefaultFixedCostAccrual 的值。
### getDefaultOvertimeRate() {#getDefaultOvertimeRate--}
```
public final double getDefaultOvertimeRate()
```


获取 DefaultOvertimeRate 的值。

**Returns:**
double - DefaultOvertimeRate 的值。
### getDefaultStandardRate() {#getDefaultStandardRate--}
```
public final double getDefaultStandardRate()
```


获取 DefaultStandardRate 的值。

**Returns:**
double - DefaultStandardRate 的值。
### getDefaultStartTime() {#getDefaultStartTime--}
```
public final Date getDefaultStartTime()
```


获取 DefaultStartTime 的值。

**Returns:**
java.util.Date - DefaultStartTime 的值。
### getDefaultTaskEVMethod() {#getDefaultTaskEVMethod--}
```
public final int getDefaultTaskEVMethod()
```


获取 DefaultTaskEVMethod 的值。

**Returns:**
int - DefaultTaskEVMethod 的值。
### getDefaultTaskType() {#getDefaultTaskType--}
```
public final int getDefaultTaskType()
```


获取 DefaultTaskType 的值。

**Returns:**
int - DefaultTaskType 的值。
### getDefaultView() {#getDefaultView--}
```
public final View getDefaultView()
```


获取项目的默认视图。

**Returns:**
[View](../../com.aspose.tasks/view) - default view of the project.
### getDefaultWeekWorkingDays() {#getDefaultWeekWorkingDays--}
```
public final WeekDayCollection getDefaultWeekWorkingDays()
```


获取 [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) 类的实例，该类表示项目默认工作周的工作日和工作时间的集合。

**Returns:**
[WeekDayCollection](../../com.aspose.tasks/weekdaycollection) - The instance of [WeekDayCollection](../../com.aspose.tasks/weekdaycollection) class which contains a list of [WeekDay](../../com.aspose.tasks/weekday) objects.

--------------------

数据仅包含在 mpp 文件中（不在 xml 中）。
### getDisplayOptions() {#getDisplayOptions--}
```
public final ProjectDisplayOptions getDisplayOptions()
```


获取 [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) 类的实例。

**Returns:**
[ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) - an instance of the [ProjectDisplayOptions](../../com.aspose.tasks/projectdisplayoptions) class.
### getDuration(double val) {#getDuration-double-}
```
public final Duration getDuration(double val)
```


获取具有指定单位数量和默认持续时间格式的 [Duration](../../com.aspose.tasks/duration) 对象，默认格式在项目设置 [Prj.DURATION\_FORMAT](../../com.aspose.tasks/prj\#DURATION-FORMAT) 中定义。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
|  | val | double | 指定数量的单位。 |

--------------------

此方法应谨慎使用，因为它根据 Project.DurationFormat 设置返回不同的持续时间。例如，当 Project.DurationFormat 为 TimeUnitType.Hour 时，GetWork(1.0) 将返回 1 小时；如果 Project.DurationFormat 为 TimeUnitType.Day，则返回 1 天。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDuration(double val, byte timeUnit) {#getDuration-double-byte-}
```
public final Duration getDuration(double val, byte timeUnit)
```


获取具有指定数量的 [TimeUnitType](../../com.aspose.tasks/timeunittype) 单位的 [Duration](../../com.aspose.tasks/duration) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| val | double | 指定数量的单位。 |
| timeUnit | 字节 | 指定的 TimeUnitType 值。 |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getDurationFormat() {#getDurationFormat--}
```
public final byte getDurationFormat()
```


获取 DurationFormat 的值。

**Returns:**
byte - DurationFormat 的值。
### getEarnedValueMethod() {#getEarnedValueMethod--}
```
public final int getEarnedValueMethod()
```


获取 EarnedValueMethod 的值。

**Returns:**
int - EarnedValueMethod 的值。
### getExtendedAttributes() {#getExtendedAttributes--}
```
public final ExtendedAttributeDefinitionCollection getExtendedAttributes()
```


获取 ExtendedAttributeDefinitionCollection 对象。与项目关联的扩展属性（自定义字段）定义集合。

**Returns:**
[ExtendedAttributeDefinitionCollection](../../com.aspose.tasks/extendedattributedefinitioncollection) - ExtendedAttributeDefinitionCollection object.
### getExtendedCreationDate() {#getExtendedCreationDate--}
```
public final Date getExtendedCreationDate()
```


获取 ExtendedCreationDate 的值。

**Returns:**
java.util.Date - ExtendedCreationDate 的值。
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


获取 FinishDate 的值。

**Returns:**
java.util.Date - FinishDate 的值。
### getFiscalYearStart() {#getFiscalYearStart--}
```
public final NullableBool getFiscalYearStart()
```


获取一个值，指示是否已设置 FiscalYearStart。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether FiscalYearStart is set or not.
### getFyStartDate() {#getFyStartDate--}
```
public final int getFyStartDate()
```


获取 FyStartDate 的值。

**Returns:**
int - FyStartDate 的值。
### getGlobalizationSettings() {#getGlobalizationSettings--}
```
public final GlobalizationSettings getGlobalizationSettings()
```


获取项目的全球化（特定语言）设置。

推荐的做法是在整个项目中使用与区域设置无关的文字或格式。但是，如果项目使用特定区域设置的文字，则可以使用此类帮助计算引擎解析这些文字。

**Returns:**
[GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) - globalization (language-specific) settings of the project.
### getGuid() {#getGuid--}
```
public final UUID getGuid()
```


获取 Guid 的值。

**Returns:**
java.util.UUID - Guid 的值。
### getHonorConstraints() {#getHonorConstraints--}
```
public final NullableBool getHonorConstraints()
```


获取一个值，指示是否已设置 HonorConstraints。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether HonorConstraints is set or not.
### getHyperlinkBase() {#getHyperlinkBase--}
```
public final String getHyperlinkBase()
```


获取 HyperlinkBase 的值。

**Returns:**
java.lang.String - HyperlinkBase 的值。
### getInsertedProjectsLikeSummary() {#getInsertedProjectsLikeSummary--}
```
public final NullableBool getInsertedProjectsLikeSummary()
```


获取一个值，指示是否已设置 InsertedProjectsLikeSummary。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether InsertedProjectsLikeSummary is set or not.
### getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled() {#getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled--}
```
public final NullableBool getKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled()
```


获取一个值，指示是否已设置 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.
### getKeywords() {#getKeywords--}
```
public final String getKeywords()
```


获取 Keywords 的值。

**Returns:**
java.lang.String - Keywords 的值。
### getLastAuthor() {#getLastAuthor--}
```
public final String getLastAuthor()
```


获取 LastAuthor 的值。

**Returns:**
java.lang.String - LastAuthor 的值。
### getLastPrinted() {#getLastPrinted--}
```
public final Date getLastPrinted()
```


获取 LastPrinted 的值。

**Returns:**
java.util.Date - LastPrinted 的值。
### getLastSaved() {#getLastSaved--}
```
public final Date getLastSaved()
```


获取 LastSaved 的值。

**Returns:**
java.util.Date - LastSaved 的值。
### getManager() {#getManager--}
```
public final String getManager()
```


获取 Manager 的值。

**Returns:**
java.lang.String - Manager 的值。
### getMicrosoftProjectServerURL() {#getMicrosoftProjectServerURL--}
```
public final NullableBool getMicrosoftProjectServerURL()
```


获取一个值，指示 MicrosoftProjectServerURL 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MicrosoftProjectServerURL is set or not.
### getMinutesPerDay() {#getMinutesPerDay--}
```
public final int getMinutesPerDay()
```


获取 MinutesPerDay 的值。

**Returns:**
int - MinutesPerDay 的值。
### getMinutesPerWeek() {#getMinutesPerWeek--}
```
public final int getMinutesPerWeek()
```


获取 MinutesPerWeek 的值。

**Returns:**
int - MinutesPerWeek 的值。
### getMoveCompletedEndsBack() {#getMoveCompletedEndsBack--}
```
public final NullableBool getMoveCompletedEndsBack()
```


获取一个值，指示 MoveCompletedEndsBack 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsBack is set or not.
### getMoveCompletedEndsForward() {#getMoveCompletedEndsForward--}
```
public final NullableBool getMoveCompletedEndsForward()
```


获取一个值，指示 MoveCompletedEndsForward 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveCompletedEndsForward is set or not.
### getMoveRemainingStartsBack() {#getMoveRemainingStartsBack--}
```
public final NullableBool getMoveRemainingStartsBack()
```


获取一个值，指示 MoveRemainingStartsBack 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsBack is set or not.
### getMoveRemainingStartsForward() {#getMoveRemainingStartsForward--}
```
public final NullableBool getMoveRemainingStartsForward()
```


获取一个值，指示 MoveRemainingStartsForward 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MoveRemainingStartsForward is set or not.
### getMultipleCriticalPaths() {#getMultipleCriticalPaths--}
```
public final NullableBool getMultipleCriticalPaths()
```


获取一个值，指示 MultipleCriticalPaths 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether MultipleCriticalPaths is set or not.
### getName() {#getName--}
```
public final String getName()
```


获取 Name 的值。

**Returns:**
java.lang.String - Name 的一个值。
### getNewTaskStartDate() {#getNewTaskStartDate--}
```
public final int getNewTaskStartDate()
```


获取 NewTaskStartDate 的值。

**Returns:**
int - NewTaskStartDate 的值。
### getNewTasksAreManual() {#getNewTasksAreManual--}
```
public final NullableBool getNewTasksAreManual()
```


获取一个值，指示 NewTasksAreManual 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksAreManual is set or not.
### getNewTasksEffortDriven() {#getNewTasksEffortDriven--}
```
public final NullableBool getNewTasksEffortDriven()
```


获取一个值，指示 NewTasksEffortDriven 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEffortDriven is set or not.
### getNewTasksEstimated() {#getNewTasksEstimated--}
```
public final NullableBool getNewTasksEstimated()
```


获取一个值，指示 NewTasksEstimated 是否已设置。

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether NewTasksEstimated is set or not.
### getOleObjects() {#getOleObjects--}
```
public final OleObjectCollection getOleObjects()
```


获取一个集合，包含链接或嵌入到此项目文件的 [OleObject](../../com.aspose/tasks/oleobject) 类实例。

--------------------

仅适用于 mpp 文件格式。此集合是只读的，除 'Clear' 操作外。

**Returns:**
[OleObjectCollection](../../com.aspose.tasks/oleobjectcollection) - a collection containing the instances of the [OleObject](../../com.aspose.tasks/oleobject) class which are linked or embedded to this project file.
### getOutlineCodes() {#getOutlineCodes--}
```
public final OutlineCodeDefinitionCollection getOutlineCodes()
```


获取 OutlineCodeDefinitionCollection 对象。与项目关联的大纲代码定义集合。

**Returns:**
[OutlineCodeDefinitionCollection](../../com.aspose.tasks/outlinecodedefinitioncollection) - OutlineCodeDefinitionCollection object.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


返回使用默认 [Timescale](../../com.aspose.tasks/timescale)（天）渲染项目的页数。

**Returns:**
int - 要渲染的页数。
### getPageCount(SaveOptions saveOptions) {#getPageCount-com.aspose.tasks.SaveOptions-}
```
public final int getPageCount(SaveOptions saveOptions)
```


返回使用给定的 [SaveOptions](../../com.aspose.tasks/saveoptions) 渲染项目的页数。

--------------------

&gt; ```
&gt; 在此示例中，HtmlSaveOptions 的实例以及生成的 HTML 页数将写入控制台。
&gt; ``````

  [C#]
Project project = new Project(@"test.mpp");
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
IncludeProjectNameInPageHeader = false,
IncludeProjectNameInTitle = false,
PageSize = PageSize.A4,
Timescale = Timescale.Days,
StartDate = project.Get(Prj.StartDate).Date,
EndDate = project.Get(Prj.FinishDate).Date
};
Console.WriteLine(project.GetPageCount(saveOptions));
  
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveOptions | [SaveOptions](../../com.aspose.tasks/saveoptions) | The save options to get page count for. |

**Returns:**
int - a page count to be rendered.
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
### getPrimaveraProperties() {#getPrimaveraProperties--}
```
public final PrimaveraProjectProperties getPrimaveraProperties()
```


Gets an object containing Primavera-specific properties for a project read from Primavera file.

**Returns:**
[PrimaveraProjectProperties](../../com.aspose.tasks/primaveraprojectproperties) - an object containing Primavera-specific properties for a project read from Primavera file.
### getProjectExternallyEdited() {#getProjectExternallyEdited--}
```
public final NullableBool getProjectExternallyEdited()
```


Gets a value indicating whether ProjectExternallyEdited is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ProjectExternallyEdited is set or not.
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
### getRemoveFileProperties() {#getRemoveFileProperties--}
```
public final NullableBool getRemoveFileProperties()
```


Gets a value indicating whether RemoveFileProperties is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether RemoveFileProperties is set or not.
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
### getRevision() {#getRevision--}
```
public final int getRevision()
```


Gets a value of Revision.

**Returns:**
int - a value of Revision.
### getRootTask() {#getRootTask--}
```
公共 最终 Task getRootTask()
```


Gets the root of the tree of tasks.

**Returns:**
[Task](../../com.aspose.tasks/task) - the root of the tree of tasks.
### getSaveVersion() {#getSaveVersion--}
```
公共 最终 int getSaveVersion()
```


Gets a value of SaveVersion.

**Returns:**
int - a value of SaveVersion.
### getScheduleFromStart() {#getScheduleFromStart--}
```
公共 最终 NullableBool getScheduleFromStart()
```


Gets a value indicating whether ScheduleFromStart is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether ScheduleFromStart is set or not.
### getShowProjectSummaryTask() {#getShowProjectSummaryTask--}
```
公共 最终 boolean getShowProjectSummaryTask()
```


Gets a value indicating whether ShowProjectSummaryTask is set or not.

**Returns:**
boolean - a value indicating whether ShowProjectSummaryTask is set or not.
### getSplitsInProgressTasks() {#getSplitsInProgressTasks--}
```
公共 最终 NullableBool getSplitsInProgressTasks()
```


Gets a value indicating whether SplitsInProgressTasks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SplitsInProgressTasks is set or not.
### getSpreadActualCost() {#getSpreadActualCost--}
```
公共 最终 NullableBool getSpreadActualCost()
```


Gets a value indicating whether SpreadActualCost is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadActualCost is set or not.
### getSpreadPercentComplete() {#getSpreadPercentComplete--}
```
公共 最终 NullableBool getSpreadPercentComplete()
```


Gets a value indicating whether SpreadPercentComplete is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether SpreadPercentComplete is set or not.
### getStartDate() {#getStartDate--}
```
公共 最终 Date getStartDate()
```


Gets a value of StartDate.

**Returns:**
java.util.Date - a value of StartDate.
### getStatusDate() {#getStatusDate--}
```
公共 最终 Date getStatusDate()
```


Gets a value of StatusDate.

**Returns:**
java.util.Date - a value of StatusDate.
### getSubject() {#getSubject--}
```
公共 最终 String getSubject()
```


Gets a value of Subject.

**Returns:**
java.lang.String - a value of Subject.
### getTables() {#getTables--}
```
公共 最终 TableCollection getTables()
```


Gets a list of [Table](../../com.aspose.tasks/table) objects.

**Returns:**
[TableCollection](../../com.aspose.tasks/tablecollection) - a list of [Table](../../com.aspose.tasks/table) objects.
### getTaskFilters() {#getTaskFilters--}
```
公共 最终 FilterCollection getTaskFilters()
```


Gets all the task-based filter definitions. TaskFilters is a collection of [Filter](../../com.aspose.tasks/filter) objects.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - all the task-based filter definitions.
### getTaskGroups() {#getTaskGroups--}
```
公共 最终 GroupCollection getTaskGroups()
```


Gets all the task-based group definitions. TaskGroups is a collection of [Group](../../com.aspose.tasks/group) objects.

**Returns:**
[GroupCollection](../../com.aspose.tasks/groupcollection) - all the task-based group definitions.
### getTaskLinks() {#getTaskLinks--}
```
公共 最终 TaskLinkCollection getTaskLinks()
```


Gets [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.

**Returns:**
[TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) - [TaskLinkCollection](../../com.aspose.tasks/tasklinkcollection) object.
### getTaskUpdatesResource() {#getTaskUpdatesResource--}
```
公共 最终 NullableBool getTaskUpdatesResource()
```


Gets a value indicating whether TaskUpdatesResource is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether TaskUpdatesResource is set or not.
### getTemplate() {#getTemplate--}
```
公共 最终 String getTemplate()
```


Gets a value of Template.

**Returns:**
java.lang.String - a value of Template.
### getTimescaleFinish() {#getTimescaleFinish--}
```
公共 最终 Date getTimescaleFinish()
```


Gets a value of TimescaleFinish.

**Returns:**
java.util.Date - a value of TimescaleFinish.
### getTimescaleStart() {#getTimescaleStart--}
```
公共 最终 Date getTimescaleStart()
```


Gets a value of TimescaleStart.

**Returns:**
java.util.Date - a value of TimescaleStart.
### getTitle() {#getTitle--}
```
公共 最终 String getTitle()
```


Gets a value of Title.

**Returns:**
java.lang.String - a value of Title.
### getUid() {#getUid--}
```
公共 最终 String getUid()
```


Gets a value of Uid.

**Returns:**
java.lang.String - a value of Uid.
### getUpdateManuallyScheduledTasksWhenEditingLinks() {#getUpdateManuallyScheduledTasksWhenEditingLinks--}
```
公共 最终 NullableBool getUpdateManuallyScheduledTasksWhenEditingLinks()
```


Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Returns:**
[NullableBool](../../com.aspose.tasks/nullablebool) - a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.
### getVbaProject() {#getVbaProject--}
```
公共 最终 VbaProject getVbaProject()
```


Gets an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.

**Returns:**
[VbaProject](../../com.aspose.tasks/vbaproject) - an instance of `VbaProject`([getVbaProject()](../../com.aspose.tasks/project\#getVbaProject--)/[setVbaProject(VbaProject)](../../com.aspose.tasks/project\#setVbaProject-VbaProject-)) class.
### getViews() {#getViews--}
```
公共 最终 ViewCollection getViews()
```


Gets a list of [View](../../com.aspose.tasks/view) objects.

**Returns:**
[ViewCollection](../../com.aspose.tasks/viewcollection) - a list of [View](../../com.aspose.tasks/view) objects.
### getWBSCodeDefinition() {#getWBSCodeDefinition--}
```
公共 最终 WBSCodeDefinition getWBSCodeDefinition()
```


Gets WBS Code Definition for the project.

**Returns:**
[WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) - WBS Code Definition for the project.
### getWeekStartDay() {#getWeekStartDay--}
```
公共 最终 int getWeekStartDay()
```


Gets a value of WeekStartDay.

**Returns:**
int - a value of WeekStartDay.
### getWork(double val) {#getWork-double-}
```
public final Duration getWork(double val)
```


Gets [Duration](../../com.aspose.tasks/duration) object with the specified `double` value and default work format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| val | double | specified double value.

--------------------

This method should be used carefully because it returns different durations depending on Project.WorkFormat setting. For example, GetWork(1.0) will return 1 hour when Project.WorkFormat is TimeUnitType.Hour or 1 day if Project.WorkFormat is TimeUnitType.Day. |

**Returns:**
[Duration](../../com.aspose.tasks/duration) - Duration object.
### getWorkFormat() {#getWorkFormat--}
```
public final byte getWorkFormat()
```


Gets a value of WorkFormat.

**Returns:**
byte - a value of WorkFormat.
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

### print(PrinterSettings printerSettings) {#print-com.aspose.tasks.PrinterSettings-}
```
public final void print(PrinterSettings printerSettings)
```


Prints project according to the specified printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerSettings | [PrinterSettings](../../com.aspose.tasks/printersettings) | the specified instance of the [PrinterSettings](../../com.aspose.tasks/printersettings) class. |

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

### print(String printerName) {#print-java.lang.String-}
```
public final void print(String printerName)
```


Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| printerName | java.lang.String | Specified printer name. |

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
| after | java.util.Date | The date to reschedule uncompleted work after. |

### rescheduleUncompletedWorkToStartAfter(Date after, List&lt;Task&gt; taskCollection) {#rescheduleUncompletedWorkToStartAfter-java.util.Date-java.util.List-com.aspose.tasks.Task--}
```
public final void rescheduleUncompletedWorkToStartAfter(Date after, List<Task> taskCollection)
```


Reschedules uncompleted work for a specified list of tasks to start after a specified date.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| after | java.util.Date | The date to reschedule uncompleted work after. |
| taskCollection | java.util.List&lt;com.aspose.tasks.Task&gt; | List&lt;Task&gt; of tasks to reschedule uncompleted work for. |

### save(OutputStream stream, SimpleSaveOptions options) {#save-java.io.OutputStream-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(OutputStream stream, SimpleSaveOptions options)
```


Saves the project to a stream using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

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

### save(String filename) {#save-java.lang.String-}
```
public final void save(String filename)
```


Saves the project data to the file in mpp format.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |

### save(String filename, SimpleSaveOptions options) {#save-java.lang.String-com.aspose.tasks.SimpleSaveOptions-}
```
public final void save(String filename, SimpleSaveOptions options)
```


Saves the document to a file using the specified save options.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filename | java.lang.String | The file name. |
| options | [SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions) | The save options. |

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

### saveAsTemplate(String fileName) {#saveAsTemplate-java.lang.String-}
```
public final void saveAsTemplate(String fileName)
```


Saves the project as a template to the specified file path.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | the specified file name. |

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

### saveReport(OutputStream stream) {#saveReport-java.io.OutputStream-}
```
public final void saveReport(OutputStream stream)
```


Saves the project overview report to the stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The stream to save project report to. |

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

### saveReport(String fileName) {#saveReport-java.lang.String-}
```
public final void saveReport(String fileName)
```


Saves the project overview report to PDF file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fileName | java.lang.String | The file name. |

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
### set(Key&lt;Date,Byte&gt; key, Date val) {#set-com.aspose.tasks.Key-java.util.Date-java.lang.Byte--java.util.Date-}
```
public final void set(Key<Date,Byte> key, Date val)
```


Maps the specified property to the specified value in this container.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | com.aspose.tasks.Key&lt;java.util.Date,java.lang.Byte&gt; | the specified property key. [Prj](../../com.aspose.tasks/prj) for getting the property key. |
| val | java.util.Date | the value. |

### setActualsInSync(NullableBool value) {#setActualsInSync-com.aspose.tasks.NullableBool-}
```
public final void setActualsInSync(NullableBool value)
```


Sets a value indicating whether ActualsInSync is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ActualsInSync is set or not. |

### setAdminProject(NullableBool value) {#setAdminProject-com.aspose.tasks.NullableBool-}
```
public final void setAdminProject(NullableBool value)
```


Sets a value indicating whether AdminProject is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AdminProject is set or not. |

### setAreEditableActualCosts(NullableBool value) {#setAreEditableActualCosts-com.aspose.tasks.NullableBool-}
```
public final void setAreEditableActualCosts(NullableBool value)
```


Sets a value indicating whether AreEditableActualCosts is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AreEditableActualCosts is set or not. |

### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public final void setAuthor(String value)
```


Sets a value of Author.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Author. |

### setAutoAddNewResourcesAndTasks(NullableBool value) {#setAutoAddNewResourcesAndTasks-com.aspose.tasks.NullableBool-}
```
public final void setAutoAddNewResourcesAndTasks(NullableBool value)
```


Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether AutoAddNewResourcesAndTasks is set or not. |

### setAutoCalculateAssignmentCosts(boolean value) {#setAutoCalculateAssignmentCosts-boolean-}
```
public final void setAutoCalculateAssignmentCosts(boolean value)
```


Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |

### setAutolink(NullableBool value) {#setAutolink-com.aspose.tasks.NullableBool-}
```
public final void setAutolink(NullableBool value)
```


Sets a value indicating whether Autolink is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether Autolink is set or not. |

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

### setBaselineForEarnedValue(int value) {#setBaselineForEarnedValue-int-}
```
public final void setBaselineForEarnedValue(int value)
```


Sets a value of BaselineForEarnedValue.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of BaselineForEarnedValue. |

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

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public final void setCalculationMode(int value)
```


Sets calculation mode of a project. Can be one of the values of `CalculationMode`([getCalculationMode()](../../com.aspose.tasks/project\#getCalculationMode--)/[setCalculationMode(int)](../../com.aspose.tasks/project\#setCalculationMode-int-)) enumeration.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | calculation mode of a project. |

### setCalendar(Calendar value) {#setCalendar-com.aspose.tasks.Calendar-}
```
public final void setCalendar(Calendar value)
```


Sets a value of Calendar.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Calendar](../../com.aspose.tasks/calendar) | a value of Calendar. |

### setCategory(String value) {#setCategory-java.lang.String-}
```
public final void setCategory(String value)
```


Sets a value of Category.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Category. |

### setComments(String value) {#setComments-java.lang.String-}
```
public final void setComments(String value)
```


Sets a value of Comments.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Comments. |

### setCompany(String value) {#setCompany-java.lang.String-}
```
public final void setCompany(String value)
```


Sets a value of Company.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Company. |

### setCreationDate(Date value) {#setCreationDate-java.util.Date-}
```
public final void setCreationDate(Date value)
```


Sets a value of CreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CreationDate. |

### setCriticalSlackLimit(int value) {#setCriticalSlackLimit-int-}
```
public final void setCriticalSlackLimit(int value)
```


Tasks are considered critical by MS Project if total slack is less or equal to this number of days.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | the maximum value of total slack time (in days) at which a task is considered critical |

### setCurrencyCode(String value) {#setCurrencyCode-java.lang.String-}
```
public final void setCurrencyCode(String value)
```


Sets a value of CurrencyCode.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencyCode. |

### setCurrencyDigits(int value) {#setCurrencyDigits-int-}
```
public final void setCurrencyDigits(int value)
```


Sets a value of CurrencyDigits.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencyDigits. |

### setCurrencySymbol(String value) {#setCurrencySymbol-java.lang.String-}
```
public final void setCurrencySymbol(String value)
```


Sets a value of CurrencySymbol.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CurrencySymbol. |

### setCurrencySymbolPosition(int value) {#setCurrencySymbolPosition-int-}
```
public final void setCurrencySymbolPosition(int value)
```


Sets a value of CurrencySymbolPosition.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of CurrencySymbolPosition. |

### setCurrentDate(Date value) {#setCurrentDate-java.util.Date-}
```
public final void setCurrentDate(Date value)
```


Sets a value of CurrentDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of CurrentDate. |

### setCustomDateFormat(String value) {#setCustomDateFormat-java.lang.String-}
```
public final void setCustomDateFormat(String value)
```


Sets a value of CustomDateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of CustomDateFormat. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Sets a value of DateFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DateFormat. |

### setDaysPerMonth(int value) {#setDaysPerMonth-int-}
```
public final void setDaysPerMonth(int value)
```


Sets a value of DaysPerMonth.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DaysPerMonth. |

### setDefaultFinishTime(Date value) {#setDefaultFinishTime-java.util.Date-}
```
public final void setDefaultFinishTime(Date value)
```


Sets a value of DefaultFinishTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultFinishTime. |

### setDefaultFixedCostAccrual(int value) {#setDefaultFixedCostAccrual-int-}
```
public final void setDefaultFixedCostAccrual(int value)
```


Sets a value of DefaultFixedCostAccrual.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultFixedCostAccrual. |

### setDefaultOvertimeRate(double value) {#setDefaultOvertimeRate-double-}
```
public final void setDefaultOvertimeRate(double value)
```


Sets a value of DefaultOvertimeRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultOvertimeRate. |

### setDefaultStandardRate(double value) {#setDefaultStandardRate-double-}
```
public final void setDefaultStandardRate(double value)
```


Sets a value of DefaultStandardRate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double | a value of DefaultStandardRate. |

### setDefaultStartTime(Date value) {#setDefaultStartTime-java.util.Date-}
```
public final void setDefaultStartTime(Date value)
```


Sets a value of DefaultStartTime.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of DefaultStartTime. |

### setDefaultTaskEVMethod(int value) {#setDefaultTaskEVMethod-int-}
```
public final void setDefaultTaskEVMethod(int value)
```


Sets a value of DefaultTaskEVMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskEVMethod. |

### setDefaultTaskType(int value) {#setDefaultTaskType-int-}
```
public final void setDefaultTaskType(int value)
```


Sets a value of DefaultTaskType.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of DefaultTaskType. |

### setDefaultView(View value) {#setDefaultView-com.aspose.tasks.View-}
```
public final void setDefaultView(View value)
```


Sets default view of the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | default view of the project. |

### setDurationFormat(byte value) {#setDurationFormat-byte-}
```
public final void setDurationFormat(byte value)
```


Sets a value of DurationFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of DurationFormat. |

### setEarnedValueMethod(int value) {#setEarnedValueMethod-int-}
```
public final void setEarnedValueMethod(int value)
```


Sets a value of EarnedValueMethod.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of EarnedValueMethod. |

### setExtendedCreationDate(Date value) {#setExtendedCreationDate-java.util.Date-}
```
public final void setExtendedCreationDate(Date value)
```


Sets a value of ExtendedCreationDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of ExtendedCreationDate. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Sets a value of FinishDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of FinishDate. |

### setFiscalYearStart(NullableBool value) {#setFiscalYearStart-com.aspose.tasks.NullableBool-}
```
public final void setFiscalYearStart(NullableBool value)
```


Sets a value indicating whether FiscalYearStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether FiscalYearStart is set or not. |

### setFyStartDate(int value) {#setFyStartDate-int-}
```
public final void setFyStartDate(int value)
```


Sets a value of FyStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of FyStartDate. |

### setGlobalizationSettings(GlobalizationSettings value) {#setGlobalizationSettings-com.aspose.tasks.GlobalizationSettings-}
```
public final void setGlobalizationSettings(GlobalizationSettings value)
```


Sets globalization (language-specific) settings of the project.

The recommended way is to use culture-invariant literals or formats throughout the project. However, if a project uses culture-specific literals, this class can be used to help the calculation engine parse those literals.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GlobalizationSettings](../../com.aspose.tasks/globalizationsettings) | globalization (language-specific) settings of the project. |

### setGuid(UUID value) {#setGuid-java.util.UUID-}
```
public final void setGuid(UUID value)
```


Sets a value of Guid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID | a value of Guid. |

### setHonorConstraints(NullableBool value) {#setHonorConstraints-com.aspose.tasks.NullableBool-}
```
public final void setHonorConstraints(NullableBool value)
```


Sets a value indicating whether HonorConstraints is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether HonorConstraints is set or not. |

### setHyperlinkBase(String value) {#setHyperlinkBase-java.lang.String-}
```
public final void setHyperlinkBase(String value)
```


Sets a value of HyperlinkBase.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of HyperlinkBase. |

### setInsertedProjectsLikeSummary(NullableBool value) {#setInsertedProjectsLikeSummary-com.aspose.tasks.NullableBool-}
```
public final void setInsertedProjectsLikeSummary(NullableBool value)
```


Sets a value indicating whether InsertedProjectsLikeSummary is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether InsertedProjectsLikeSummary is set or not. |

### setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value) {#setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled-com.aspose.tasks.NullableBool-}
```
public final void setKeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled(NullableBool value)
```


Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |

### setKeywords(String value) {#setKeywords-java.lang.String-}
```
public final void setKeywords(String value)
```


Sets a value of Keywords.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Keywords. |

### setLastAuthor(String value) {#setLastAuthor-java.lang.String-}
```
public final void setLastAuthor(String value)
```


Sets a value of LastAuthor.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of LastAuthor. |

### setLastPrinted(Date value) {#setLastPrinted-java.util.Date-}
```
public final void setLastPrinted(Date value)
```


Sets a value of LastPrinted.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastPrinted. |

### setLastSaved(Date value) {#setLastSaved-java.util.Date-}
```
public final void setLastSaved(Date value)
```


Sets a value of LastSaved.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of LastSaved. |

### setManager(String value) {#setManager-java.lang.String-}
```
public final void setManager(String value)
```


Sets a value of Manager.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Manager. |

### setMicrosoftProjectServerURL(NullableBool value) {#setMicrosoftProjectServerURL-com.aspose.tasks.NullableBool-}
```
public final void setMicrosoftProjectServerURL(NullableBool value)
```


Sets a value indicating whether MicrosoftProjectServerURL is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MicrosoftProjectServerURL is set or not. |

### setMinutesPerDay(int value) {#setMinutesPerDay-int-}
```
public final void setMinutesPerDay(int value)
```


Sets a value of MinutesPerDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerDay. |

### setMinutesPerWeek(int value) {#setMinutesPerWeek-int-}
```
public final void setMinutesPerWeek(int value)
```


Sets a value of MinutesPerWeek.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of MinutesPerWeek. |

### setMoveCompletedEndsBack(NullableBool value) {#setMoveCompletedEndsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsBack(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsBack is set or not. |

### setMoveCompletedEndsForward(NullableBool value) {#setMoveCompletedEndsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveCompletedEndsForward(NullableBool value)
```


Sets a value indicating whether MoveCompletedEndsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveCompletedEndsForward is set or not. |

### setMoveRemainingStartsBack(NullableBool value) {#setMoveRemainingStartsBack-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsBack(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsBack is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsBack is set or not. |

### setMoveRemainingStartsForward(NullableBool value) {#setMoveRemainingStartsForward-com.aspose.tasks.NullableBool-}
```
public final void setMoveRemainingStartsForward(NullableBool value)
```


Sets a value indicating whether MoveRemainingStartsForward is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MoveRemainingStartsForward is set or not. |

### setMultipleCriticalPaths(NullableBool value) {#setMultipleCriticalPaths-com.aspose.tasks.NullableBool-}
```
public final void setMultipleCriticalPaths(NullableBool value)
```


Sets a value indicating whether MultipleCriticalPaths is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether MultipleCriticalPaths is set or not. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Sets a value of Name.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Name. |

### setNewTaskStartDate(int value) {#setNewTaskStartDate-int-}
```
public final void setNewTaskStartDate(int value)
```


Sets a value of NewTaskStartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of NewTaskStartDate. |

### setNewTasksAreManual(NullableBool value) {#setNewTasksAreManual-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksAreManual(NullableBool value)
```


Sets a value indicating whether NewTasksAreManual is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksAreManual is set or not. |

### setNewTasksEffortDriven(NullableBool value) {#setNewTasksEffortDriven-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEffortDriven(NullableBool value)
```


Sets a value indicating whether NewTasksEffortDriven is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEffortDriven is set or not. |

### setNewTasksEstimated(NullableBool value) {#setNewTasksEstimated-com.aspose.tasks.NullableBool-}
```
public final void setNewTasksEstimated(NullableBool value)
```


Sets a value indicating whether NewTasksEstimated is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether NewTasksEstimated is set or not. |

### setProjectExternallyEdited(NullableBool value) {#setProjectExternallyEdited-com.aspose.tasks.NullableBool-}
```
public final void setProjectExternallyEdited(NullableBool value)
```


Sets a value indicating whether ProjectExternallyEdited is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ProjectExternallyEdited is set or not. |

### setRemoveFileProperties(NullableBool value) {#setRemoveFileProperties-com.aspose.tasks.NullableBool-}
```
public final void setRemoveFileProperties(NullableBool value)
```


Sets a value indicating whether RemoveFileProperties is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether RemoveFileProperties is set or not. |

### setRevision(int value) {#setRevision-int-}
```
public final void setRevision(int value)
```


Sets a value of Revision.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of Revision. |

### setSaveVersion(int value) {#setSaveVersion-int-}
```
public final void setSaveVersion(int value)
```


Sets a value of SaveVersion.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of SaveVersion. |

### setScheduleFromStart(NullableBool value) {#setScheduleFromStart-com.aspose.tasks.NullableBool-}
```
public final void setScheduleFromStart(NullableBool value)
```


Sets a value indicating whether ScheduleFromStart is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether ScheduleFromStart is set or not. |

### setShowProjectSummaryTask(boolean value) {#setShowProjectSummaryTask-boolean-}
```
public final void setShowProjectSummaryTask(boolean value)
```


Sets a value indicating whether ShowProjectSummaryTask is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | a value indicating whether ShowProjectSummaryTask is set or not. |

### setSplitsInProgressTasks(NullableBool value) {#setSplitsInProgressTasks-com.aspose.tasks.NullableBool-}
```
public final void setSplitsInProgressTasks(NullableBool value)
```


Sets a value indicating whether SplitsInProgressTasks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SplitsInProgressTasks is set or not. |

### setSpreadActualCost(NullableBool value) {#setSpreadActualCost-com.aspose.tasks.NullableBool-}
```
public final void setSpreadActualCost(NullableBool value)
```


Sets a value indicating whether SpreadActualCost is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadActualCost is set or not. |

### setSpreadPercentComplete(NullableBool value) {#setSpreadPercentComplete-com.aspose.tasks.NullableBool-}
```
public final void setSpreadPercentComplete(NullableBool value)
```


Sets a value indicating whether SpreadPercentComplete is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether SpreadPercentComplete is set or not. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Sets a value of StartDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StartDate. |

### setStatusDate(Date value) {#setStatusDate-java.util.Date-}
```
public final void setStatusDate(Date value)
```


Sets a value of StatusDate.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of StatusDate. |

### setSubject(String value) {#setSubject-java.lang.String-}
```
public final void setSubject(String value)
```


Sets a value of Subject.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Subject. |

### setTaskUpdatesResource(NullableBool value) {#setTaskUpdatesResource-com.aspose.tasks.NullableBool-}
```
public final void setTaskUpdatesResource(NullableBool value)
```


Sets a value indicating whether TaskUpdatesResource is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether TaskUpdatesResource is set or not. |

### setTemplate(String value) {#setTemplate-java.lang.String-}
```
public final void setTemplate(String value)
```


Sets a value of Template.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Template. |

### setTimescaleFinish(Date value) {#setTimescaleFinish-java.util.Date-}
```
public final void setTimescaleFinish(Date value)
```


Sets a value of TimescaleFinish.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleFinish. |

### setTimescaleStart(Date value) {#setTimescaleStart-java.util.Date-}
```
public final void setTimescaleStart(Date value)
```


Sets a value of TimescaleStart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.Date | a value of TimescaleStart. |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public final void setTitle(String value)
```


Sets a value of Title.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Title. |

### setUid(String value) {#setUid-java.lang.String-}
```
public final void setUid(String value)
```


Sets a value of Uid.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String | a value of Uid. |

### setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value) {#setUpdateManuallyScheduledTasksWhenEditingLinks-com.aspose.tasks.NullableBool-}
```
public final void setUpdateManuallyScheduledTasksWhenEditingLinks(NullableBool value)
```


Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [NullableBool](../../com.aspose.tasks/nullablebool) | a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |

### setWBSCodeDefinition(WBSCodeDefinition value) {#setWBSCodeDefinition-com.aspose.tasks.WBSCodeDefinition-}
```
public final void setWBSCodeDefinition(WBSCodeDefinition value)
```


Sets WBS Code Definition for the project.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [WBSCodeDefinition](../../com.aspose.tasks/wbscodedefinition) | WBS Code Definition for the project. |

### setWeekStartDay(int value) {#setWeekStartDay-int-}
```
public final void setWeekStartDay(int value)
```


Sets a value of WeekStartDay.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int | a value of WeekStartDay. |

### setWorkFormat(byte value) {#setWorkFormat-byte-}
```
public final void setWorkFormat(byte value)
```


Sets a value of WorkFormat.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte | a value of WorkFormat. |

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

