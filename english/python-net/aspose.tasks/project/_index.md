---
title: Project
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 810
url: /python-net/aspose.tasks/project/
---

## Project class

Represents a project.

The Project type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|Project()|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class.|
|Project(project_template, protection_password)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from a password protected template (existent mpp or mpt file).|
|Project(project_template)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from a password protected template (existent mpp or mpt file).|
|Project(stream, options)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from the Stream<br/>            with the specified instance of the [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) class.|
|Project(stream)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from the Stream<br/>            with the specified instance of the [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) class.|
|Project(project_template, options)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from a template (existent MPP or MPT file) <br/>            with the specified instance of the [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) class.|
|Project(settings)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class to read data from a database which is specified by the instance of the [DbSettings](/tasks/python-net/aspose.tasks.connectivity/dbsettings/) class.|
|Project(stream, protection_password)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from a template(existent mpp or mpt file).|
|Project(project_template, options)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from a template (existent mpp or mpt file)<br/>            with the specified instance of the [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) class.|
|Project(stream, options)|Initializes a new instance of the [Project](/tasks/python-net/aspose.tasks/project/) class from the Stream<br/>            with the specified instance of the [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) class.|
## Properties
| Name | Description |
| :- | :- |
|actuals_in_sync|Gets or sets a value indicating whether ActualsInSync is set or not.|
|admin_project|Gets or sets a value indicating whether AdminProject is set or not.|
|are_editable_actual_costs|Gets or sets a value indicating whether AreEditableActualCosts is set or not.|
|author|Gets or sets a value of Author.|
|auto_add_new_resources_and_tasks|Gets or sets a value indicating whether AutoAddNewResourcesAndTasks is set or not.|
|autolink|Gets or sets a value indicating whether Autolink is set or not.|
|baseline_for_earned_value|Gets or sets a value of BaselineForEarnedValue.|
|calendar|Gets or sets a value of Calendar.|
|category|Gets or sets a value of Category.|
|comments|Gets or sets a value of Comments.|
|company|Gets or sets a value of Company.|
|creation_date|Gets or sets a value of CreationDate.|
|critical_slack_limit|Tasks are considered critical by MS Project if total slack is less or equal to this number of days.|
|currency_code|Gets or sets a value of CurrencyCode.|
|currency_digits|Gets or sets a value of CurrencyDigits.|
|currency_symbol|Gets or sets a value of CurrencySymbol.|
|currency_symbol_position|Gets or sets a value of CurrencySymbolPosition.|
|current_date|Gets or sets a value of CurrentDate.|
|date_format|Gets or sets a value of DateFormat.|
|custom_date_format|Gets or sets a value of CustomDateFormat.|
|days_per_month|Gets or sets a value of DaysPerMonth.|
|default_finish_time|Gets or sets a value of DefaultFinishTime.|
|default_fixed_cost_accrual|Gets or sets a value of DefaultFixedCostAccrual.|
|default_overtime_rate|Gets or sets a value of DefaultOvertimeRate.|
|default_standard_rate|Gets or sets a value of DefaultStandardRate.|
|default_start_time|Gets or sets a value of DefaultStartTime.|
|default_task_ev_method|Gets or sets a value of DefaultTaskEVMethod.|
|default_task_type|Gets or sets a value of DefaultTaskType.|
|duration_format|Gets or sets a value of DurationFormat.|
|earned_value_method|Gets or sets a value of EarnedValueMethod.|
|extended_creation_date|Gets or sets a value of ExtendedCreationDate.|
|finish_date|Gets or sets a value of FinishDate.|
|fiscal_year_start|Gets or sets a value indicating whether FiscalYearStart is set or not.|
|fy_start_date|Gets or sets a value of FyStartDate.|
|honor_constraints|Gets or sets a value indicating whether HonorConstraints is set or not.|
|hyperlink_base|Gets or sets a value of HyperlinkBase.|
|inserted_projects_like_summary|Gets or sets a value indicating whether InsertedProjectsLikeSummary is set or not.|
|keep_task_on_nearest_working_time_when_made_auto_scheduled|Gets or sets a value indicating whether KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled is set or not.|
|keywords|Gets or sets a value of Keywords.|
|last_author|Gets or sets a value of LastAuthor.|
|last_printed|Gets or sets a value of LastPrinted.|
|last_saved|Gets or sets a value of LastSaved.|
|manager|Gets or sets a value of Manager.|
|microsoft_project_server_url|Gets or sets a value indicating whether MicrosoftProjectServerURL is set or not.|
|minutes_per_day|Gets or sets a value of MinutesPerDay.|
|minutes_per_week|Gets or sets a value of MinutesPerWeek.|
|move_completed_ends_back|Gets or sets a value indicating whether MoveCompletedEndsBack is set or not.|
|move_completed_ends_forward|Gets or sets a value indicating whether MoveCompletedEndsForward is set or not.|
|move_remaining_starts_back|Gets or sets a value indicating whether MoveRemainingStartsBack is set or not.|
|move_remaining_starts_forward|Gets or sets a value indicating whether MoveRemainingStartsForward is set or not.|
|multiple_critical_paths|Gets or sets a value indicating whether MultipleCriticalPaths is set or not.|
|name|Gets or sets a value of Name.|
|new_tasks_are_manual|Gets or sets a value indicating whether NewTasksAreManual is set or not.|
|new_tasks_effort_driven|Gets or sets a value indicating whether NewTasksEffortDriven is set or not.|
|new_tasks_estimated|Gets or sets a value indicating whether NewTasksEstimated is set or not.|
|new_task_start_date|Gets or sets a value of NewTaskStartDate.|
|project_externally_edited|Gets or sets a value indicating whether ProjectExternallyEdited is set or not.|
|remove_file_properties|Gets or sets a value indicating whether RemoveFileProperties is set or not.|
|revision|Gets or sets a value of Revision.|
|save_version|Gets or sets a value of SaveVersion.|
|schedule_from_start|Gets or sets a value indicating whether ScheduleFromStart is set or not.|
|show_project_summary_task|Gets or sets a value indicating whether ShowProjectSummaryTask is set or not.|
|splits_in_progress_tasks|Gets or sets a value indicating whether SplitsInProgressTasks is set or not.|
|spread_actual_cost|Gets or sets a value indicating whether SpreadActualCost is set or not.|
|spread_percent_complete|Gets or sets a value indicating whether SpreadPercentComplete is set or not.|
|start_date|Gets or sets a value of StartDate.|
|status_date|Gets or sets a value of StatusDate.|
|subject|Gets or sets a value of Subject.|
|task_updates_resource|Gets or sets a value indicating whether TaskUpdatesResource is set or not.|
|template|Gets or sets a value of Template.|
|timescale_finish|Gets or sets a value of TimescaleFinish.|
|timescale_start|Gets or sets a value of TimescaleStart.|
|title|Gets or sets a value of Title.|
|uid|Gets or sets a value of Uid.|
|update_manually_scheduled_tasks_when_editing_links|Gets or sets a value indicating whether UpdateManuallyScheduledTasksWhenEditingLinks is set or not.|
|week_start_day|Gets or sets a value of WeekStartDay.|
|work_format|Gets or sets a value of WorkFormat.|
|guid|Gets or sets a value of Guid.|
|auto_calculate_assignment_costs|Gets or sets whether assignment cost and remaining cost should be auto calculated using assignment's work and resource rates.|
|default_view|Gets or sets default view of the project.|
|vba_project|Gets an instance of [vba_project](/tasks/python-net/aspose.tasks/project/) class.|
|display_options|Gets an instance of the [ProjectDisplayOptions](/tasks/python-net/aspose.tasks/projectdisplayoptions/) class.|
|calculation_mode|Gets or sets calculation mode of a project.<br/>            Can be one of the values of [calculation_mode](/tasks/python-net/aspose.tasks/project/) enumeration.|
|root_task|Gets the root of the tree of tasks.|
|task_links|Gets [TaskLinkCollection](/tasks/python-net/aspose.tasks/tasklinkcollection/) object.|
|calendars|Gets [CalendarCollection](/tasks/python-net/aspose.tasks/calendarcollection/) object of this Project instance.|
|resources|Gets ResourceCollection object.|
|outline_codes|Gets OutlineCodeDefinitionCollection object.<br/>            The collection of outline code definitions associated with a project.|
|resource_assignments|Gets ResourceAssignmentCollection object.|
|default_week_working_days|Gets the instance of [WeekDayCollection](/tasks/python-net/aspose.tasks/weekdaycollection/) class which represents a collection of project default week working days and working times.|
|built_in_props|Gets project's built-in properties collection.|
|custom_props|Gets project's custom properties collection.|
|extended_attributes|Gets ExtendedAttributeDefinitionCollection object.<br/>            The collection of extended attribute (custom fields) definitions associated with a project.|
|critical_path|Gets a collection which contains a list of Critical tasks which comprise Critical Path of this project.|
|task_filters|Gets all the task-based filter definitions. <br/>            TaskFilters is a collection of [Filter](/tasks/python-net/aspose.tasks/filter/) objects.|
|resource_filters|Gets all the resource-based filter definitions. <br/>            ResourceFilters is a collection of [Filter](/tasks/python-net/aspose.tasks/filter/) objects.|
|views|Gets a list of [View](/tasks/python-net/aspose.tasks/view/) objects.|
|tables|Gets a list of [Table](/tasks/python-net/aspose.tasks/table/) objects.|
|task_groups|Gets all the task-based group definitions. <br/>            TaskGroups is a collection of [Group](/tasks/python-net/aspose.tasks/group/) objects.|
|resource_groups|Gets all of the resource-based group definitions. <br/>            ResourceGroups is a collection of [Group](/tasks/python-net/aspose.tasks/group/) objects.|
|wbs_code_definition|Gets or sets WBS Code Definition for the project.|
|ole_objects|Gets a collection containing the instances of the [OleObject](/tasks/python-net/aspose.tasks/oleobject/) class which are linked or embedded to this project file.|
|primavera_properties|Gets an object containing Primavera-specific properties for a project read from Primavera file.|
## Methods
| Name | Description |
| :- | :- |
|get_project_file_info(filename)|Read project file info from the file.|
|get_project_file_info(stream)|Gets project file info from the stream.|
|recalculate()|Recalculates Start and Finish of resources.|
|recalculate(validate)|Reschedules all project tasks ids, outline levels, start/finish dates, sets early/late dates, calculates slacks, work and cost fields with optional validation.|
|save(filename, options)|Saves the document to a file using the specified save options.|
|save(filename, format)|Saves the project data to the file.|
|save(filename)|Saves the document to a file using the specified save options.|
|save(stream, options)|Saves the project to a stream using the specified save options.|
|save(stream, format)|Saves the project data to the stream.|
|save_report(stream)|Saves the project overview report to the stream.|
|save_report(file_name)|Saves the project overview report to PDF file.|
|save_report(stream, report_type)|Saves the project report of the specified type to the specified stream.|
|save_report(file_name, report_type)|Saves the project report of the specified type in PDF format to the specified file path.|
|save_as_template(file_name, options)|Saves the project as a template.|
|save_as_template(file_name)|Saves the project as a template.|
|save_as_template(stream)|Saves the project as a template to a specified stream.|
|save_as_template(stream, options)|Saves the project as a template to a specified stream.|
|get_page_count(save_options)|Returns page count for the project to be rendered using given [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/).|
|get_page_count()|Returns page count for the project to be rendered using given [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/).|
|get_page_count(scale)|Returns page count for the project to be rendered using given [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/).|
|get_page_count(format)|Returns page count for the project to be rendered using default [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)(Days) and given [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/)|
|get_page_count(format, scale)|Returns page count for the project to be rendered using given [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/) and [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/).|
|get_page_count(page_size, scale, start_date, end_date)|Returns page count for the project to be rendered using given [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/), [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) and date range.|
|get_page_count(page_size, scale)|Returns page count for the project to be rendered using given [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/), [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) and date range.|
|copy_to(another)|Copies project's main data and properties to another project.|
|copy_to(another, options)|Copies project's main data and properties to another project.|
|print()|Prints project to the default printer with default printer settings using the standard (no User Interface) print controller.|
|print(options)|Prints project to the default printer with default printer settings and custom save options using the standard (no User Interface) print controller.|
|print(printer_name)|Prints project to the specified printer with default printer settings using the standard (no User Interface) print controller.|
|print(printer_settings)|Prints project according to the specified printer settings using the standard (no User Interface) print controller.|
|print(printer_settings, document_name)|Prints project according to the specified printer settings using the standard (no User Interface) print controller.|
|print(printer_settings, options)|Prints project according to the specified printer settings and custom save options using the standard (no User Interface) print controller.|
|print(printer_settings, options, document_name)|Prints project according to the specified printer settings, custom save options and the specified document name using the standard (no User Interface) print controller.|
|set_baseline(baseline_type)|Sets the baseline save time.|
|set_baseline(baseline_type, task_collection)|  |
|update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only)|Updates all work as complete through a specified date for the entire project.|
|update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only, task_collection)|  |
|reschedule_uncompleted_work_to_start_after(after)|Reschedules uncompleted project work to start after a specified date.|
|reschedule_uncompleted_work_to_start_after(after, task_collection)|  |
|renumber_wbs_code()|Renumber WBS code of all tasks.|
|renumber_wbs_code(task_ids)|  |
|get_duration(val)|Gets [Duration](/tasks/python-net/aspose.tasks/duration/) object with the specified number of units and default duration format which is defined in project's settings [None](/tasks/python-net/aspose.tasks/prj/).|
|get_duration(val, time_unit)|Gets [Duration](/tasks/python-net/aspose.tasks/duration/) object with the specified number of [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) units.|
|get_duration(time_span, time_unit)|Gets [Duration](/tasks/python-net/aspose.tasks/duration/) object with the specified datatime value and specified [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) value.|
|select_all_child_tasks()|Recursively collects all child tasks of the root task.|
|enumerate_all_child_tasks()|Recursively enumerates all project's tasks including root task.|
|get_predecessors(task)|Returns a collection of task links which are predecessors of the specified task.|
|recalculate_resource_start_finish()|Recalculates Start and Finish of resources.|
|recalculate_resource_fields()|Recalculates Id, Start and Finish of resources.|
|remove_invalid_resource_assignments()|Eliminates invalid resource assignments from the project resource assignments list.|
|get_baseline_save_time(baseline_number)|Returns the baseline save time.|
|set_baseline_save_time(baseline_number, value)|Sets the baseline save time.|
|get_work(val)|Gets [Duration](/tasks/python-net/aspose.tasks/duration/) object with the specified float value and default work format.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

