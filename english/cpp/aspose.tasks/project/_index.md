---
title: "Aspose::Tasks::Project class"
linktitle: "Project"
articleTitle: "Project"
second_title: "Aspose.Tasks for C++"
description: "Represents a project."
type: docs
weight: 10
url: /cpp/aspose.tasks/project/
---

## Project class

Represents a project.

The Project is a central class in the Aspose.Tasks library.

One can use Project to read one of supported project management formats: MPP, MPT, MPX, XML.

To load an existing document in any of the supported formats, pass a file name or a stream into one of the Project constructors. To create a blank project, call the parameterless constructor.

Use one of the Save method overloads to save the project in any of the Aspose::Tasks::Saving::SaveFileFormat formats: Primavera: P6 XML, PM XER; Microsoft Excel: XLSX, XML; Fixed Layout: PDF; Images: JPEG, PNG, BMP, TIFF, SVG; Text: TXT; Others: HTML.

The Project stores project-wide information such as Aspose::Tasks::Project::Views , Aspose::Tasks::Project::BuiltInProps , Aspose::Tasks::Project::CustomProps , and Aspose::Tasks::Project::ExtendedAttributes . Most of these objects are accessible via the corresponding properties of the Project class.

The Project is a root entity that contains entry points to manipulate other project entities, such as Aspose::Tasks::Task , Aspose::Tasks::Resource , Aspose::Tasks::ResourceAssignment , Aspose::Tasks::ExtendedAttribute and Aspose::Tasks::Calendar .

The Project entities can be accessed via typed collections, for example Aspose::Tasks::Task::Children , Aspose::Tasks::Project::Resources , Aspose::Tasks::Project::ResourceAssignments , etc.

## Constructors

| Name | Description |
| --- | --- |
| [Project (13 overloads)](./project/) | Initializes a new instance of the Project class. |

## Methods

| Name | Description |
| --- | --- |
| [CopyTo (2 overloads)](./copyto/) | Copies project's main data and properties to another project. |
| [EnumerateAllChildTasks](./enumerateallchildtasks/) | Recursively enumerates all project's tasks including root task. |
| [Get](./get/) | Returns the value to which the property is mapped in this container. |
| [get_ActualsInSync](./get_actualsinsync/) | Gets a value indicating whether ActualsInSync is set or not. |
| [get_AdminProject](./get_adminproject/) | Gets a value indicating whether AdminProject is set or not. |
| [get_AreEditableActualCosts](./get_areeditableactualcosts/) | Gets a value indicating whether AreEditableActualCosts is set or not. |
| [get_Author](./get_author/) | Gets a value of Author. |
| [get_AutoAddNewResourcesAndTasks](./get_autoaddnewresourcesandtasks/) | Gets a value indicating whether AutoAddNewResourcesAndTasks is set or not. |
| [get_AutoCalculateAssignmentCosts](./get_autocalculateassignmentcosts/) | Gets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |
| [get_Autolink](./get_autolink/) | Gets a value indicating whether Autolink is set or not. |
| [get_BaselineForEarnedValue](./get_baselineforearnedvalue/) | Gets a value of BaselineForEarnedValue. |
| [get_BuiltInProps](./get_builtinprops/) | Gets project's built-in properties collection. |
| [get_CalculationMode](./get_calculationmode/) | Gets calculation mode of a project. Can be one of the values of CalculationMode enumeration. |
| [get_Calendar](./get_calendar/) | Gets a value of Calendar . |
| [get_Calendars](./get_calendars/) | Gets CalendarCollection object of this Project instance. |
| [get_Category](./get_category/) | Gets a value of Category. |
| [get_Comments](./get_comments/) | Gets a value of Comments. |
| [get_Company](./get_company/) | Gets a value of Company. |
| [get_CreationDate](./get_creationdate/) | Gets a value of CreationDate. |
| [get_CriticalPath](./get_criticalpath/) | Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project. |
| [get_CriticalSlackLimit](./get_criticalslacklimit/) | Gets a value of CriticalSlackLimit. |
| [get_CurrencyCode](./get_currencycode/) | Gets a value of CurrencyCode. |
| [get_CurrencyDigits](./get_currencydigits/) | Gets a value of CurrencyDigits. |
| [get_CurrencySymbol](./get_currencysymbol/) | Gets a value of CurrencySymbol. |
| [get_CurrencySymbolPosition](./get_currencysymbolposition/) | Gets a value of CurrencySymbolPosition. |
| [get_CurrentDate](./get_currentdate/) | Gets a value of CurrentDate. |
| [get_CustomDateFormat](./get_customdateformat/) | Gets a value of CustomDateFormat. |
| [get_CustomProps](./get_customprops/) | Gets project's custom properties collection. |
| [get_DateFormat](./get_dateformat/) | Gets a value of DateFormat. |
| [get_DaysPerMonth](./get_dayspermonth/) | Gets a value of DaysPerMonth. |
| [get_DefaultFinishTime](./get_defaultfinishtime/) | Gets a value of DefaultFinishTime. |
| [get_DefaultFixedCostAccrual](./get_defaultfixedcostaccrual/) | Gets a value of DefaultFixedCostAccrual. |
| [get_DefaultOvertimeRate](./get_defaultovertimerate/) | Gets a value of DefaultOvertimeRate. |
| [get_DefaultStandardRate](./get_defaultstandardrate/) | Gets a value of DefaultStandardRate. |
| [get_DefaultStartTime](./get_defaultstarttime/) | Gets a value of DefaultStartTime. |
| [get_DefaultTaskEVMethod](./get_defaulttaskevmethod/) | Gets a value of DefaultTaskEVMethod. |
| [get_DefaultTaskType](./get_defaulttasktype/) | Gets a value of DefaultTaskType. |
| [get_DefaultView](./get_defaultview/) | Gets default view of the project. |
| [get_DefaultWeekWorkingDays](./get_defaultweekworkingdays/) | Gets the instance of WeekDayCollection class which represents a collection of project default week working days and working times. |
| [get_DisplayOptions](./get_displayoptions/) | Gets an instance of the ProjectDisplayOptions class. |
| [get_DurationFormat](./get_durationformat/) | Gets a value of DurationFormat. |
| [get_EarnedValueMethod](./get_earnedvaluemethod/) | Gets a value of EarnedValueMethod. |
| [get_ExtendedAttributes](./get_extendedattributes/) | Gets ExtendedAttributeDefinitionCollection object. The collection of extended attribute (custom fields) definitions associated with a project. |
| [get_ExtendedCreationDate](./get_extendedcreationdate/) | Gets a value of ExtendedCreationDate. |
| [get_FinishDate](./get_finishdate/) | Gets a value of FinishDate. |
| [get_FiscalYearStart](./get_fiscalyearstart/) | Gets a value indicating whether FiscalYearStart is set or not. |
| [get_FyStartDate](./get_fystartdate/) | Gets a value of FyStartDate. |
| [get_Guid](./get_guid/) | Gets a value of Guid. |
| [get_HonorConstraints](./get_honorconstraints/) | Gets a value indicating whether HonorConstraints is set or not. |
| [get_HyperlinkBase](./get_hyperlinkbase/) | Gets a value of HyperlinkBase. |
| [get_InsertedProjectsLikeSummary](./get_insertedprojectslikesummary/) | Gets a value indicating whether InsertedProjectsLikeSummary is set or not. |
| [get_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./get_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Gets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |
| [get_Keywords](./get_keywords/) | Gets a value of Keywords. |
| [get_LastAuthor](./get_lastauthor/) | Gets a value of LastAuthor. |
| [get_LastPrinted](./get_lastprinted/) | Gets a value of LastPrinted. |
| [get_LastSaved](./get_lastsaved/) | Gets a value of LastSaved. |
| [get_Manager](./get_manager/) | Gets a value of Manager. |
| [get_MicrosoftProjectServerURL](./get_microsoftprojectserverurl/) | Gets a value indicating whether MicrosoftProjectServerURL is set or not. |
| [get_MinutesPerDay](./get_minutesperday/) | Gets a value of MinutesPerDay. |
| [get_MinutesPerWeek](./get_minutesperweek/) | Gets a value of MinutesPerWeek. |
| [get_MoveCompletedEndsBack](./get_movecompletedendsback/) | Gets a value indicating whether MoveCompletedEndsBack is set or not. |
| [get_MoveCompletedEndsForward](./get_movecompletedendsforward/) | Gets a value indicating whether MoveCompletedEndsForward is set or not. |
| [get_MoveRemainingStartsBack](./get_moveremainingstartsback/) | Gets a value indicating whether MoveRemainingStartsBack is set or not. |
| [get_MoveRemainingStartsForward](./get_moveremainingstartsforward/) | Gets a value indicating whether MoveRemainingStartsForward is set or not. |
| [get_MultipleCriticalPaths](./get_multiplecriticalpaths/) | Gets a value indicating whether MultipleCriticalPaths is set or not. |
| [get_Name](./get_name/) | Gets a value of Name. |
| [get_NewTasksAreManual](./get_newtasksaremanual/) | Gets a value indicating whether NewTasksAreManual is set or not. |
| [get_NewTasksEffortDriven](./get_newtaskseffortdriven/) | Gets a value indicating whether NewTasksEffortDriven is set or not. |
| [get_NewTasksEstimated](./get_newtasksestimated/) | Gets a value indicating whether NewTasksEstimated is set or not. |
| [get_NewTaskStartDate](./get_newtaskstartdate/) | Gets a value of NewTaskStartDate. |
| [get_OleObjects](./get_oleobjects/) | Gets a collection containing the instances of the OleObject class which are linked or embedded to this project file. |
| [get_OutlineCodes](./get_outlinecodes/) | Gets OutlineCodeDefinitionCollection object. The collection of outline code definitions associated with a project. |
| [get_PrimaveraProperties](./get_primaveraproperties/) | Gets an object containing Primavera-specific properties for a project read from Primavera file. |
| [get_ProjectExternallyEdited](./get_projectexternallyedited/) | Gets a value indicating whether ProjectExternallyEdited is set or not. |
| [get_RemoveFileProperties](./get_removefileproperties/) | Gets a value indicating whether RemoveFileProperties is set or not. |
| [get_ResourceAssignments](./get_resourceassignments/) | Gets ResourceAssignmentCollection object. |
| [get_ResourceFilters](./get_resourcefilters/) | Gets all the resource-based filter definitions. ResourceFilters is a collection of Filter objects. |
| [get_ResourceGroups](./get_resourcegroups/) | Gets all of the resource-based group definitions. ResourceGroups is a collection of Group objects. |
| [get_Resources](./get_resources/) | Gets ResourceCollection object. |
| [get_Revision](./get_revision/) | Gets a value of Revision. |
| [get_RootTask](./get_roottask/) | Gets the root of the tree of tasks. |
| [get_SaveVersion](./get_saveversion/) | Gets a value of SaveVersion. |
| [get_ScheduleFromStart](./get_schedulefromstart/) | Gets a value indicating whether ScheduleFromStart is set or not. |
| [get_ShowProjectSummaryTask](./get_showprojectsummarytask/) | Gets a value indicating whether ShowProjectSummaryTask is set or not. |
| [get_SplitsInProgressTasks](./get_splitsinprogresstasks/) | Gets a value indicating whether SplitsInProgressTasks is set or not. |
| [get_SpreadActualCost](./get_spreadactualcost/) | Gets a value indicating whether SpreadActualCost is set or not. |
| [get_SpreadPercentComplete](./get_spreadpercentcomplete/) | Gets a value indicating whether SpreadPercentComplete is set or not. |
| [get_StartDate](./get_startdate/) | Gets a value of StartDate. |
| [get_StatusDate](./get_statusdate/) | Gets a value of StatusDate. |
| [get_Subject](./get_subject/) | Gets a value of Subject. |
| [get_Tables](./get_tables/) | Gets a list of Table objects. |
| [get_TaskFilters](./get_taskfilters/) | Gets all the task-based filter definitions. TaskFilters is a collection of Filter objects. |
| [get_TaskGroups](./get_taskgroups/) | Gets all the task-based group definitions. TaskGroups is a collection of Group objects. |
| [get_TaskLinks](./get_tasklinks/) | Gets TaskLinkCollection object. |
| [get_TaskUpdatesResource](./get_taskupdatesresource/) | Gets a value indicating whether TaskUpdatesResource is set or not. |
| [get_Template](./get_template/) | Gets a value of Template. |
| [get_TimescaleFinish](./get_timescalefinish/) | Gets a value of TimescaleFinish. |
| [get_TimescaleStart](./get_timescalestart/) | Gets a value of TimescaleStart. |
| [get_Title](./get_title/) | Gets a value of Title. |
| [get_Uid](./get_uid/) | Gets a value of Uid. |
| [get_UpdateManuallyScheduledTasksWhenEditingLinks](./get_updatemanuallyscheduledtaskswheneditinglinks/) | Gets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |
| [get_VbaProject](./get_vbaproject/) | Gets an instance of VbaProject class. |
| [get_Views](./get_views/) | Gets a list of View objects. |
| [get_WBSCodeDefinition](./get_wbscodedefinition/) | Gets WBS Code Definition for the project. |
| [get_WeekStartDay](./get_weekstartday/) | Gets a value of WeekStartDay. |
| [get_WorkFormat](./get_workformat/) | Gets a value of WorkFormat. |
| [GetBaselineSaveTime](./getbaselinesavetime/) | Returns the baseline save time. |
| [GetDuration (3 overloads)](./getduration/) | Gets Duration object with the specified number of units and default duration format which is defined in project's settings Prj::DurationFormat . |
| [GetPageCount (7 overloads)](./getpagecount/) | Returns page count for the project to be rendered using default Timescale (Days). |
| [GetPredecessors](./getpredecessors/) | Returns a collection of task links which are predecessors of the specified task. |
| [GetProjectFileInfo (2 overloads)](./getprojectfileinfo/) | Gets project file info from the stream. |
| [GetWork](./getwork/) | Gets Duration object with the specified double value and default work format. |
| [Recalculate (2 overloads)](./recalculate/) | Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields. |
| [RecalculateResourceFields](./recalculateresourcefields/) | Recalculates Id, Start and Finish of resources. |
| [RecalculateResourceStartFinish](./recalculateresourcestartfinish/) | Recalculates Start and Finish of resources. |
| [RemoveInvalidResourceAssignments](./removeinvalidresourceassignments/) | Eliminates invalid resource assignments from the project resource assignments list. |
| [RenumberWBSCode (2 overloads)](./renumberwbscode/) | Renumber WBS code of all tasks. |
| [RescheduleUncompletedWorkToStartAfter (2 overloads)](./rescheduleuncompletedworktostartafter/) | Reschedules uncompleted project work to start after a specified date. |
| [Save (5 overloads)](./save/) | Saves the project to a stream using the specified save options. |
| [SaveAsTemplate (4 overloads)](./saveastemplate/) | Saves the project as a template to a specified stream. |
| [SaveReport (4 overloads)](./savereport/) | Saves the project overview report to the stream. |
| [SelectAllChildTasks](./selectallchildtasks/) | Recursively collects all child tasks of the root task. |
| [Set (2 overloads)](./set/) | Maps the specified property to the specified value in this container. |
| [set_ActualsInSync](./set_actualsinsync/) | Sets a value indicating whether ActualsInSync is set or not. |
| [set_AdminProject](./set_adminproject/) | Sets a value indicating whether AdminProject is set or not. |
| [set_AreEditableActualCosts](./set_areeditableactualcosts/) | Sets a value indicating whether AreEditableActualCosts is set or not. |
| [set_Author](./set_author/) | Sets a value of Author. |
| [set_AutoAddNewResourcesAndTasks](./set_autoaddnewresourcesandtasks/) | Sets a value indicating whether AutoAddNewResourcesAndTasks is set or not. |
| [set_AutoCalculateAssignmentCosts](./set_autocalculateassignmentcosts/) | Sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates. |
| [set_Autolink](./set_autolink/) | Sets a value indicating whether Autolink is set or not. |
| [set_BaselineForEarnedValue](./set_baselineforearnedvalue/) | Sets a value of BaselineForEarnedValue. |
| [set_CalculationMode](./set_calculationmode/) | Sets calculation mode of a project. Can be one of the values of CalculationMode enumeration. |
| [set_Calendar](./set_calendar/) | Sets a value of Calendar . |
| [set_Category](./set_category/) | Sets a value of Category. |
| [set_Comments](./set_comments/) | Sets a value of Comments. |
| [set_Company](./set_company/) | Sets a value of Company. |
| [set_CreationDate](./set_creationdate/) | Sets a value of CreationDate. |
| [set_CriticalSlackLimit](./set_criticalslacklimit/) | Sets a value of CriticalSlackLimit. |
| [set_CurrencyCode](./set_currencycode/) | Sets a value of CurrencyCode. |
| [set_CurrencyDigits](./set_currencydigits/) | Sets a value of CurrencyDigits. |
| [set_CurrencySymbol](./set_currencysymbol/) | Sets a value of CurrencySymbol. |
| [set_CurrencySymbolPosition](./set_currencysymbolposition/) | Sets a value of CurrencySymbolPosition. |
| [set_CurrentDate](./set_currentdate/) | Sets a value of CurrentDate. |
| [set_CustomDateFormat](./set_customdateformat/) | Sets a value of CustomDateFormat. |
| [set_DateFormat](./set_dateformat/) | Sets a value of DateFormat. |
| [set_DaysPerMonth](./set_dayspermonth/) | Sets a value of DaysPerMonth. |
| [set_DefaultFinishTime](./set_defaultfinishtime/) | Sets a value of DefaultFinishTime. |
| [set_DefaultFixedCostAccrual](./set_defaultfixedcostaccrual/) | Sets a value of DefaultFixedCostAccrual. |
| [set_DefaultOvertimeRate](./set_defaultovertimerate/) | Sets a value of DefaultOvertimeRate. |
| [set_DefaultStandardRate](./set_defaultstandardrate/) | Sets a value of DefaultStandardRate. |
| [set_DefaultStartTime](./set_defaultstarttime/) | Sets a value of DefaultStartTime. |
| [set_DefaultTaskEVMethod](./set_defaulttaskevmethod/) | Sets a value of DefaultTaskEVMethod. |
| [set_DefaultTaskType](./set_defaulttasktype/) | Sets a value of DefaultTaskType. |
| [set_DefaultView](./set_defaultview/) | Sets default view of the project. |
| [set_DurationFormat](./set_durationformat/) | Sets a value of DurationFormat. |
| [set_EarnedValueMethod](./set_earnedvaluemethod/) | Sets a value of EarnedValueMethod. |
| [set_ExtendedCreationDate](./set_extendedcreationdate/) | Sets a value of ExtendedCreationDate. |
| [set_FinishDate](./set_finishdate/) | Sets a value of FinishDate. |
| [set_FiscalYearStart](./set_fiscalyearstart/) | Sets a value indicating whether FiscalYearStart is set or not. |
| [set_FyStartDate](./set_fystartdate/) | Sets a value of FyStartDate. |
| [set_Guid](./set_guid/) | Sets a value of Guid. |
| [set_HonorConstraints](./set_honorconstraints/) | Sets a value indicating whether HonorConstraints is set or not. |
| [set_HyperlinkBase](./set_hyperlinkbase/) | Sets a value of HyperlinkBase. |
| [set_InsertedProjectsLikeSummary](./set_insertedprojectslikesummary/) | Sets a value indicating whether InsertedProjectsLikeSummary is set or not. |
| [set_KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled](./set_keeptaskonnearestworkingtimewhenmadeautoscheduled/) | Sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not. |
| [set_Keywords](./set_keywords/) | Sets a value of Keywords. |
| [set_LastAuthor](./set_lastauthor/) | Sets a value of LastAuthor. |
| [set_LastPrinted](./set_lastprinted/) | Sets a value of LastPrinted. |
| [set_LastSaved](./set_lastsaved/) | Sets a value of LastSaved. |
| [set_Manager](./set_manager/) | Sets a value of Manager. |
| [set_MicrosoftProjectServerURL](./set_microsoftprojectserverurl/) | Sets a value indicating whether MicrosoftProjectServerURL is set or not. |
| [set_MinutesPerDay](./set_minutesperday/) | Sets a value of MinutesPerDay. |
| [set_MinutesPerWeek](./set_minutesperweek/) | Sets a value of MinutesPerWeek. |
| [set_MoveCompletedEndsBack](./set_movecompletedendsback/) | Sets a value indicating whether MoveCompletedEndsBack is set or not. |
| [set_MoveCompletedEndsForward](./set_movecompletedendsforward/) | Sets a value indicating whether MoveCompletedEndsForward is set or not. |
| [set_MoveRemainingStartsBack](./set_moveremainingstartsback/) | Sets a value indicating whether MoveRemainingStartsBack is set or not. |
| [set_MoveRemainingStartsForward](./set_moveremainingstartsforward/) | Sets a value indicating whether MoveRemainingStartsForward is set or not. |
| [set_MultipleCriticalPaths](./set_multiplecriticalpaths/) | Sets a value indicating whether MultipleCriticalPaths is set or not. |
| [set_Name](./set_name/) | Sets a value of Name. |
| [set_NewTasksAreManual](./set_newtasksaremanual/) | Sets a value indicating whether NewTasksAreManual is set or not. |
| [set_NewTasksEffortDriven](./set_newtaskseffortdriven/) | Sets a value indicating whether NewTasksEffortDriven is set or not. |
| [set_NewTasksEstimated](./set_newtasksestimated/) | Sets a value indicating whether NewTasksEstimated is set or not. |
| [set_NewTaskStartDate](./set_newtaskstartdate/) | Sets a value of NewTaskStartDate. |
| [set_ProjectExternallyEdited](./set_projectexternallyedited/) | Sets a value indicating whether ProjectExternallyEdited is set or not. |
| [set_RemoveFileProperties](./set_removefileproperties/) | Sets a value indicating whether RemoveFileProperties is set or not. |
| [set_Revision](./set_revision/) | Sets a value of Revision. |
| [set_SaveVersion](./set_saveversion/) | Sets a value of SaveVersion. |
| [set_ScheduleFromStart](./set_schedulefromstart/) | Sets a value indicating whether ScheduleFromStart is set or not. |
| [set_ShowProjectSummaryTask](./set_showprojectsummarytask/) | Sets a value indicating whether ShowProjectSummaryTask is set or not. |
| [set_SplitsInProgressTasks](./set_splitsinprogresstasks/) | Sets a value indicating whether SplitsInProgressTasks is set or not. |
| [set_SpreadActualCost](./set_spreadactualcost/) | Sets a value indicating whether SpreadActualCost is set or not. |
| [set_SpreadPercentComplete](./set_spreadpercentcomplete/) | Sets a value indicating whether SpreadPercentComplete is set or not. |
| [set_StartDate](./set_startdate/) | Sets a value of StartDate. |
| [set_StatusDate](./set_statusdate/) | Sets a value of StatusDate. |
| [set_Subject](./set_subject/) | Sets a value of Subject. |
| [set_TaskUpdatesResource](./set_taskupdatesresource/) | Sets a value indicating whether TaskUpdatesResource is set or not. |
| [set_Template](./set_template/) | Sets a value of Template. |
| [set_TimescaleFinish](./set_timescalefinish/) | Sets a value of TimescaleFinish. |
| [set_TimescaleStart](./set_timescalestart/) | Sets a value of TimescaleStart. |
| [set_Title](./set_title/) | Sets a value of Title. |
| [set_Uid](./set_uid/) | Sets a value of Uid. |
| [set_UpdateManuallyScheduledTasksWhenEditingLinks](./set_updatemanuallyscheduledtaskswheneditinglinks/) | Sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not. |
| [set_WBSCodeDefinition](./set_wbscodedefinition/) | Sets WBS Code Definition for the project. |
| [set_WeekStartDay](./set_weekstartday/) | Sets a value of WeekStartDay. |
| [set_WorkFormat](./set_workformat/) | Sets a value of WorkFormat. |
| [SetBaseline (2 overloads)](./setbaseline/) | Saves baseline fields to the specified baseline for the entire project. |
| [SetBaselineSaveTime](./setbaselinesavetime/) | Sets the baseline save time. |
| [UpdateProjectWorkAsComplete (2 overloads)](./updateprojectworkascomplete/) | Updates all work as complete through a specified date for the entire project. |

