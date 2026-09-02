---
title: "Aspose::Tasks::Project 类"
linktitle: "项目"
articleTitle: "项目"
second_title: "Aspose.Tasks for C++"
description: "表示一个项目。"
type: docs
weight: 10
url: /zh/cpp/aspose.tasks/project/
---

## Project class

表示一个项目。

Project 是 Aspose.Tasks 库中的核心类。

可以使用 Project 读取受支持的项目管理格式之一：MPP、MPT、MPX、XML。

要在任意受支持的格式中加载现有文档，请将文件名或流传递给其中一个 Project 构造函数。要创建空白项目，请调用无参数构造函数。

使用 Save 方法的重载之一，将项目保存为任意 Aspose::Tasks::Saving::SaveFileFormat 格式：Primavera：P6 XML、PM XER；Microsoft Excel：XLSX、XML；固定布局：PDF；图像：JPEG、PNG、BMP、TIFF、SVG；文本：TXT；其他：HTML。

Project 存储项目范围的信息，例如 Aspose::Tasks::Project::Views、Aspose::Tasks::Project::BuiltInProps、Aspose::Tasks::Project::CustomProps 和 Aspose::Tasks::Project::ExtendedAttributes。大多数这些对象可通过 Project 类的相应属性访问。

Project 是根实体，包含用于操作其他项目实体的入口点，例如 Aspose::Tasks::Task、Aspose::Tasks::Resource、Aspose::Tasks::ResourceAssignment、Aspose::Tasks::ExtendedAttribute 和 Aspose::Tasks::Calendar。

可以通过类型化集合访问 Project 实体，例如 Aspose::Tasks::Task::Children、Aspose::Tasks::Project::Resources、Aspose::Tasks::Project::ResourceAssignments 等。

## 构造函数

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [Project (13 overloads)](./project/) | 初始化 Project 类的新实例。 |

## 方法

| 表示 ResourceAssignment 对象的属性。 | Aspose::Tasks 命名空间提供核心类和枚举，用于在 C++ 中管理项目数据、资源、分配和基线信息。 |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | 将项目的主要数据和属性复制到另一个项目。 |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | 递归枚举项目的所有任务，包括根任务。 |
| [Get](./get/) | 返回属性在此容器中映射的值。 |
| [get_ActualsInSync](./get_actualsinsync/) | 获取一个值，指示 ActualsInSync 是否已设置。 |
| [get_AdminProject](./get_adminproject/) | 获取一个值，指示 AdminProject 是否已设置。 |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | 获取一个值，指示 AreEditableActualCosts 是否已设置。 |
| [get_Author](./get_author/) | 获取 Author 的值。 |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | 获取一个值，指示 AutoAddNewResourcesAndTasks 是否已设置。 |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | 获取是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| [get_Autolink](./get_autolink/) | 获取一个值，指示 Autolink 是否已设置。 |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | 获取 BaselineForEarnedValue 的值。 |
| [get_BuiltInProps](./get_builtinprops/) | 获取项目的内置属性集合。 |
| [get_CalculationMode](./get_calculationmode/) | 获取项目的计算模式。可以是 CalculationMode 枚举的其中一个值。 |
| [get_Calendar](./get_calendar/) | 获取 Calendar 的值。 |
| [get_Calendars](./get_calendars/) | 获取此 Project 实例的 CalendarCollection 对象。 |
| [get_Category](./get_category/) | 获取 Category 的值。 |
| [get_Comments](./get_comments/) | 获取 Comments 的值。 |
| [get_Company](./get_company/) | 获取 Company 的值。 |
| [get_CreationDate](./get_creationdate/) | 获取 CreationDate 的值。 |
| [get_CriticalPath](./get_criticalpath/) | 获取一个集合，其中包含构成此项目关键路径的关键任务列表。 |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | 获取 CriticalSlackLimit 的值。 |
| [get_CurrencyCode](./get_currencycode/) | 获取 CurrencyCode 的值。 |
| [get_CurrencyDigits](./get_currencydigits/) | 获取 CurrencyDigits 的值。 |
| [get_CurrencySymbol](./get_currencysymbol/) | 获取 CurrencySymbol 的值。 |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | 获取 CurrencySymbolPosition 的值。 |
| [get_CurrentDate](./get_currentdate/) | 获取 CurrentDate 的值。 |
| [get_CustomDateFormat](./get_customdateformat/) | 获取 CustomDateFormat 的值。 |
| [get_CustomProps](./get_customprops/) | 获取项目的自定义属性集合。 |
| [get_DateFormat](./get_dateformat/) | 获取 DateFormat 的值。 |
| [get_DaysPerMonth](./get_dayspermonth/) | 获取 DaysPerMonth 的值。 |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | 获取 DefaultFinishTime 的值。 |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | 获取 DefaultFixedCostAccrual 的值。 |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | 获取 DefaultOvertimeRate 的值。 |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | 获取 DefaultStandardRate 的值。 |
| [get_DefaultStartTime](./get_defaultstarttime/) | 获取 DefaultStartTime 的值。 |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | 获取 DefaultTaskEVMethod 的值。 |
| [get_DefaultTaskType](./get_defaulttasktype/) | 获取 DefaultTaskType 的值。 |
| [get_DefaultView](./get_defaultview/) | 获取项目的默认视图。 |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | 获取 WeekDayCollection 类的实例，该实例表示项目默认工作周的工作日和工作时间的集合。 |
| [get_DisplayOptions](./get_displayoptions/) | 获取 ProjectDisplayOptions 类的实例。 |
| [get_DurationFormat](./get_durationformat/) | 获取 DurationFormat 的值。 |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | 获取 EarnedValueMethod 的值。 |
| [get_ExtendedAttributes](./get_extendedattributes/) | 获取 ExtendedAttributeDefinitionCollection 对象。该集合是与项目关联的扩展属性（自定义字段）定义的集合。 |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | 获取 ExtendedCreationDate 的值。 |
| [get_FinishDate](./get_finishdate/) | 获取 FinishDate 的值。 |
| [get_FiscalYearStart](./get_fiscalyearstart/) | 获取一个值，指示 FiscalYearStart 是否已设置。 |
| [get_FyStartDate](./get_fystartdate/) | 获取 FyStartDate 的值。 |
| [get_Guid](./get_guid/) | 获取 Guid 的值。 |
| [get_HonorConstraints](./get_honorconstraints/) | 获取一个值，指示 HonorConstraints 是否已设置。 |
| [get_HyperlinkBase](./get_hyperlinkbase/) | 获取 HyperlinkBase 的值。 |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | 获取一个值，指示 InsertedProjectsLikeSummary 是否已设置。 |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | 获取一个值，指示 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 是否已设置。 |
| [get_Keywords](./get_keywords/) | 获取 Keywords 的值。 |
| [get_LastAuthor](./get_lastauthor/) | 获取 LastAuthor 的值。 |
| [get_LastPrinted](./get_lastprinted/) | 获取 LastPrinted 的值。 |
| [get_LastSaved](./get_lastsaved/) | 获取 LastSaved 的值。 |
| [get_Manager](./get_manager/) | 获取 Manager 的值。 |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | 获取一个值，指示 MicrosoftProjectServerURL 是否已设置。 |
| [get_MinutesPerDay](./get_minutesperday/) | 获取 MinutesPerDay 的值。 |
| [get_MinutesPerWeek](./get_minutesperweek/) | 获取 MinutesPerWeek 的值。 |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | 获取一个值，指示 MoveCompletedEndsBack 是否已设置。 |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | 获取一个值，指示 MoveCompletedEndsForward 是否已设置。 |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | 获取一个值，指示 MoveRemainingStartsBack 是否已设置。 |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | 获取一个值，指示 MoveRemainingStartsForward 是否已设置。 |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | 获取一个值，指示 MultipleCriticalPaths 是否已设置。 |
| [get_Name](./get_name/) | 获取 Name 的值。 |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | 获取一个值，指示 NewTasksAreManual 是否已设置。 |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | 获取一个值，指示 NewTasksEffortDriven 是否已设置。 |
| [get_NewTasksEstimated](./get_newtasksestimated/) | 获取一个值，指示 NewTasksEstimated 是否已设置。 |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | 获取 NewTaskStartDate 的值。 |
| [get_OleObjects](./get_oleobjects/) | 获取一个集合，其中包含链接或嵌入到此项目文件的 OleObject 类实例。 |
| [get_OutlineCodes](./get_outlinecodes/) | 获取 OutlineCodeDefinitionCollection 对象。该集合包含与项目关联的大纲代码定义。 |
| [get_PrimaveraProperties](./get_primaveraproperties/) | 获取一个包含从 Primavera 文件读取的项目的 Primavera 特定属性的对象。 |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | 获取一个指示是否已设置 ProjectExternallyEdited 的值。 |
| [get_RemoveFileProperties](./get_removefileproperties/) | 获取一个指示是否已设置 RemoveFileProperties 的值。 |
| [get_ResourceAssignments](./get_resourceassignments/) | 获取 ResourceAssignmentCollection 对象。 |
| [get_ResourceFilters](./get_resourcefilters/) | 获取所有基于资源的过滤器定义。ResourceFilters 是 Filter 对象的集合。 |
| [get_ResourceGroups](./get_resourcegroups/) | 获取所有基于资源的组定义。ResourceGroups 是 Group 对象的集合。 |
| [get_Resources](./get_resources/) | 获取 ResourceCollection 对象。 |
| [get_Revision](./get_revision/) | 获取 Revision 的值。 |
| [get_RootTask](./get_roottask/) | 获取任务树的根节点。 |
| [get_SaveVersion](./get_saveversion/) | 获取 SaveVersion 的值。 |
| [get_ScheduleFromStart](./get_schedulefromstart/) | 获取一个指示是否已设置 ScheduleFromStart 的值。 |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | 获取一个指示是否已设置 ShowProjectSummaryTask 的值。 |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | 获取一个指示是否已设置 SplitsInProgressTasks 的值。 |
| [get_SpreadActualCost](./get_spreadactualcost/) | 获取一个指示是否已设置 SpreadActualCost 的值。 |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | 获取一个指示是否已设置 SpreadPercentComplete 的值。 |
| [get_StartDate](./get_startdate/) | 获取 StartDate 的值。 |
| [get_StatusDate](./get_statusdate/) | 获取 StatusDate 的值。 |
| [get_Subject](./get_subject/) | 获取 Subject 的值。 |
| [get_Tables](./get_tables/) | 获取 Table 对象的列表。 |
| [get_TaskFilters](./get_taskfilters/) | 获取所有基于任务的过滤器定义。TaskFilters 是 Filter 对象的集合。 |
| [get_TaskGroups](./get_taskgroups/) | 获取所有基于任务的组定义。TaskGroups 是 Group 对象的集合。 |
| [get_TaskLinks](./get_tasklinks/) | 获取 TaskLinkCollection 对象。 |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | 获取一个指示是否已设置 TaskUpdatesResource 的值。 |
| [get_Template](./get_template/) | 获取 Template 的值。 |
| [get_TimescaleFinish](./get_timescalefinish/) | 获取 TimescaleFinish 的值。 |
| [get_TimescaleStart](./get_timescalestart/) | 获取 TimescaleStart 的值。 |
| [get_Title](./get_title/) | 获取 Title 的值。 |
| [get_Uid](./get_uid/) | 获取 Uid 的值。 |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | 获取一个值，指示 UpdateManuallyScheduledTasksWhenEditingLinks 是否已设置。 |
| [get_VbaProject](./get_vbaproject/) | 获取 VbaProject 类的实例。 |
| [get_Views](./get_views/) | 获取 View 对象的列表。 |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | 获取项目的 WBS Code Definition。 |
| [get_WeekStartDay](./get_weekstartday/) | 获取 WeekStartDay 的值。 |
| [get_WorkFormat](./get_workformat/) | 获取 WorkFormat 的值。 |
| [GetBaselineSaveTime](./getbaselinesavetime/) | 返回基线保存时间。 |
| [GetDuration (3 overloads)](./getduration/) | 获取具有指定单位数和默认持续时间格式的 Duration 对象，默认持续时间格式在项目的设置 Prj::DurationFormat 中定义。 |
| [GetPageCount (7 overloads)](./getpagecount/) | 返回使用默认 Timescale（天）渲染的项目的页数。 |
| [GetPredecessors](./getpredecessors/) | 返回指定任务的前置任务链接集合。 |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | 从流中获取项目文件信息。 |
| [GetWork](./getwork/) | 获取具有指定双精度值和默认工作格式的 Duration 对象。 |
| [Recalculate (2 overloads)](./recalculate/) | 重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算时差、工作和成本字段。 |
| [RecalculateResourceFields](./recalculateresourcefields/) | 重新计算资源的 Id、开始和结束。 |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | 重新计算资源的开始和结束。 |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | 从项目资源分配列表中消除无效的资源分配。 |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | 重新编号所有任务的 WBS 代码。 |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | 重新安排未完成的项目工作，使其在指定日期之后开始。 |
| [Save (5 overloads)](./save/) | 使用指定的保存选项将项目保存到流中。 |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | 将项目作为模板保存到指定的流中。 |
| [SaveReport (4 overloads)](./savereport/) | 将项目概览报告保存到流中。 |
| [SelectAllChildTasks](./selectallchildtasks/) | 递归收集根任务的所有子任务。 |
| [Set (2 overloads)](./set/) | 将指定属性映射到此容器中的指定值。 |
| [set_ActualsInSync](./set_actualsinsync/) | 设置一个值，指示 ActualsInSync 是否已设置。 |
| [set_AdminProject](./set_adminproject/) | 设置一个值，指示 AdminProject 是否已设置。 |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | 设置一个值，指示 AreEditableActualCosts 是否已设置。 |
| [set_Author](./set_author/) | 设置 Author 的值。 |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | 设置一个值，指示 AutoAddNewResourcesAndTasks 是否已设置。 |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | 设置是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| [set_Autolink](./set_autolink/) | 设置一个值，指示 Autolink 是否已设置。 |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | 设置 BaselineForEarnedValue 的值。 |
| [set_CalculationMode](./set_calculationmode/) | 设置项目的计算模式。可以是 CalculationMode 枚举的其中一个值。 |
| [set_Calendar](./set_calendar/) | 设置 Calendar 的值。 |
| [set_Category](./set_category/) | 设置 Category 的值。 |
| [set_Comments](./set_comments/) | 设置 Comments 的值。 |
| [set_Company](./set_company/) | 设置 Company 的值。 |
| [set_CreationDate](./set_creationdate/) | 设置 CreationDate 的值。 |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | 设置 CriticalSlackLimit 的值。 |
| [set_CurrencyCode](./set_currencycode/) | 设置 CurrencyCode 的值。 |
| [set_CurrencyDigits](./set_currencydigits/) | 设置 CurrencyDigits 的值。 |
| [set_CurrencySymbol](./set_currencysymbol/) | 设置 CurrencySymbol 的值。 |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | 设置 CurrencySymbolPosition 的值。 |
| [set_CurrentDate](./set_currentdate/) | 设置 CurrentDate 的值。 |
| [set_CustomDateFormat](./set_customdateformat/) | 设置 CustomDateFormat 的值。 |
| [set_DateFormat](./set_dateformat/) | 设置 DateFormat 的值。 |
| [set_DaysPerMonth](./set_dayspermonth/) | 设置 DaysPerMonth 的值。 |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | 设置 DefaultFinishTime 的值。 |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | 设置 DefaultFixedCostAccrual 的值。 |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | 设置 DefaultOvertimeRate 的值。 |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | 设置 DefaultStandardRate 的值。 |
| [set_DefaultStartTime](./set_defaultstarttime/) | 设置 DefaultStartTime 的值。 |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | 设置 DefaultTaskEVMethod 的值。 |
| [set_DefaultTaskType](./set_defaulttasktype/) | 设置 DefaultTaskType 的值。 |
| [set_DefaultView](./set_defaultview/) | 设置项目的默认视图。 |
| [set_DurationFormat](./set_durationformat/) | 设置 DurationFormat 的值。 |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | 设置 EarnedValueMethod 的值。 |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | 设置 ExtendedCreationDate 的值。 |
| [set_FinishDate](./set_finishdate/) | 设置 FinishDate 的值。 |
| [set_FiscalYearStart](./set_fiscalyearstart/) | 设置一个指示 FiscalYearStart 是否已设置的值。 |
| [set_FyStartDate](./set_fystartdate/) | 设置 FyStartDate 的值。 |
| [set_Guid](./set_guid/) | 设置 Guid 的值。 |
| [set_HonorConstraints](./set_honorconstraints/) | 设置一个指示 HonorConstraints 是否已设置的值。 |
| [set_HyperlinkBase](./set_hyperlinkbase/) | 设置 HyperlinkBase 的值。 |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | 设置一个指示 InsertedProjectsLikeSummary 是否已设置的值。 |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | 设置一个指示 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 是否已设置的值。 |
| [set_Keywords](./set_keywords/) | 设置 Keywords 的值。 |
| [set_LastAuthor](./set_lastauthor/) | 设置 LastAuthor 的值。 |
| [set_LastPrinted](./set_lastprinted/) | 设置 LastPrinted 的值。 |
| [set_LastSaved](./set_lastsaved/) | 设置 LastSaved 的值。 |
| [set_Manager](./set_manager/) | 设置 Manager 的值。 |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | 设置一个指示 MicrosoftProjectServerURL 是否已设置的值。 |
| [set_MinutesPerDay](./set_minutesperday/) | 设置 MinutesPerDay 的值。 |
| [set_MinutesPerWeek](./set_minutesperweek/) | 设置 MinutesPerWeek 的值。 |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | 设置一个指示 MoveCompletedEndsBack 是否已设置的值。 |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | 设置一个指示 MoveCompletedEndsForward 是否已设置的值。 |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | 设置一个指示 MoveRemainingStartsBack 是否已设置的值。 |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | 设置一个值，指示 MoveRemainingStartsForward 是否已设置. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | 设置一个值，指示 MultipleCriticalPaths 是否已设置. |
| [set_Name](./set_name/) | 设置 Name 的值。 |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | 设置一个值，指示 NewTasksAreManual 是否已设置. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | 设置一个值，指示 NewTasksEffortDriven 是否已设置. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | 设置一个值，指示 NewTasksEstimated 是否已设置. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | 设置 NewTaskStartDate 的值. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | 设置一个值，指示 ProjectExternallyEdited 是否已设置. |
| [set_RemoveFileProperties](./set_removefileproperties/) | 设置一个值，指示 RemoveFileProperties 是否已设置. |
| [set_Revision](./set_revision/) | 设置 Revision 的值. |
| [set_SaveVersion](./set_saveversion/) | 设置 SaveVersion 的值. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | 设置一个值，指示 ScheduleFromStart 是否已设置. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | 设置一个值，指示 ShowProjectSummaryTask 是否已设置. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | 设置一个值，指示 SplitsInProgressTasks 是否已设置. |
| [set_SpreadActualCost](./set_spreadactualcost/) | 设置一个值，指示 SpreadActualCost 是否已设置. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | 设置一个值，指示 SpreadPercentComplete 是否已设置. |
| [set_StartDate](./set_startdate/) | 设置 StartDate 的值. |
| [set_StatusDate](./set_statusdate/) | 设置 StatusDate 的值. |
| [set_Subject](./set_subject/) | 设置 Subject 的值. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | 设置一个值，指示 TaskUpdatesResource 是否已设置. |
| [set_Template](./set_template/) | 设置 Template 的值. |
| [set_TimescaleFinish](./set_timescalefinish/) | 设置 TimescaleFinish 的值. |
| [set_TimescaleStart](./set_timescalestart/) | 设置 TimescaleStart 的值. |
| [set_Title](./set_title/) | 设置 Title 的值. |
| [set_Uid](./set_uid/) | 设置 Uid 的值。 |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | 设置一个值，指示 UpdateManuallyScheduledTasksWhenEditingLinks 是否已设置. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | 为项目设置 WBS Code Definition. |
| [set_WeekStartDay](./set_weekstartday/) | 设置 WeekStartDay 的值。 |
| [set_WorkFormat](./set_workformat/) | 设置 WorkFormat 的值。 |
| [SetBaseline (2 overloads)](./setbaseline/) | 将基线字段保存到整个项目的指定基线。 |
| [SetBaselineSaveTime](./setbaselinesavetime/) | 设置基线保存时间。 |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | 将整个项目的所有工作更新为截至指定日期的已完成状态。 |

