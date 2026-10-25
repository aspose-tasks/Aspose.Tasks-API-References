---
title: "项目"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 810
url: /zh/python-net/aspose.tasks/project/
---

## Project class

表示一个项目。

Project 类型公开以下成员：
## 构造函数
| 名称 | 描述 |
| :- | :- |
| Project() | 初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例。 |
| Project(project_template, protection_password) | 从受密码保护的模板（现有的 mpp 或 mpt 文件）初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例。 |
| Project(project_template) | 从受密码保护的模板（现有的 mpp 或 mpt 文件）初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例。 |
| Project(stream, options) | 从流中初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例<br/>            使用指定的 [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) 类实例。 |
| Project(stream) | 从流中初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例<br/>            使用指定的 [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) 类实例。 |
| Project(project_template, options) | 从模板（现有的 MPP 或 MPT 文件）初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例 <br/>            使用指定的 [PrimaveraReadOptions](/tasks/python-net/aspose.tasks/primaverareadoptions/) 类实例。 |
| Project(settings) | 初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例，以读取由 [DbSettings](/tasks/python-net/aspose.tasks.connectivity/dbsettings/) 类实例指定的数据库中的数据。 |
| Project(stream, protection_password) | 从模板（现有的 mpp 或 mpt 文件）初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例。 |
| Project(project_template, options) | 从模板（现有的 mpp 或 mpt 文件）初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例<br/>            使用指定的 [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) 类实例。 |
| Project(stream, options) | 从流中初始化一个新的 [Project](/tasks/python-net/aspose.tasks/project/) 类实例<br/>            使用指定的 [LoadOptions](/tasks/python-net/aspose.tasks/loadoptions/) 类实例。 |
## 属性
| 名称 | 描述 |
| :- | :- |
| actuals_in_sync | 获取或设置一个值，指示 ActualsInSync 是否已设置。 |
| admin_project | 获取或设置一个值，指示 AdminProject 是否已设置。 |
| are_editable_actual_costs | 获取或设置一个值，指示 AreEditableActualCosts 是否已设置。 |
| author | 获取或设置 Author 的值。 |
| auto_add_new_resources_and_tasks | 获取或设置一个值，指示是否已设置 AutoAddNewResourcesAndTasks。 |
| autolink | 获取或设置一个值，指示是否已设置 Autolink。 |
| baseline_for_earned_value | 获取或设置 BaselineForEarnedValue 的值。 |
| calendar | 获取或设置 Calendar 的值。 |
| category | 获取或设置 Category 的值。 |
| comments | 获取或设置 Comments 的值。 |
| company | 获取或设置 Company 的值。 |
| creation_date | 获取或设置 CreationDate 的值。 |
| critical_slack_limit | 如果总浮动小于或等于此天数，MS Project 将任务视为关键任务。 |
| currency_code | 获取或设置 CurrencyCode 的值。 |
| currency_digits | 获取或设置 CurrencyDigits 的值。 |
| currency_symbol | 获取或设置 CurrencySymbol 的值。 |
| currency_symbol_position | 获取或设置 CurrencySymbolPosition 的值。 |
| current_date | 获取或设置 CurrentDate 的值。 |
| date_format | 获取或设置 DateFormat 的值。 |
| custom_date_format | 获取或设置 CustomDateFormat 的值。 |
| days_per_month | 获取或设置 DaysPerMonth 的值。 |
| default_finish_time | 获取或设置 DefaultFinishTime 的值。 |
| default_fixed_cost_accrual | 获取或设置 DefaultFixedCostAccrual 的值。 |
| default_overtime_rate | 获取或设置 DefaultOvertimeRate 的值。 |
| default_standard_rate | 获取或设置 DefaultStandardRate 的值。 |
| default_start_time | 获取或设置 DefaultStartTime 的值。 |
| default_task_ev_method | 获取或设置 DefaultTaskEVMethod 的值。 |
| default_task_type | 获取或设置 DefaultTaskType 的值。 |
| duration_format | 获取或设置 DurationFormat 的值。 |
| earned_value_method | 获取或设置 EarnedValueMethod 的值。 |
| extended_creation_date | 获取或设置 ExtendedCreationDate 的值。 |
| finish_date | 获取或设置 FinishDate 的值。 |
| fiscal_year_start | 获取或设置一个值，指示 FiscalYearStart 是否已设置。 |
| fy_start_date | 获取或设置 FyStartDate 的值。 |
| honor_constraints | 获取或设置一个值，指示 HonorConstraints 是否已设置。 |
| hyperlink_base | 获取或设置 HyperlinkBase 的值。 |
| inserted_projects_like_summary | 获取或设置一个值，指示 InsertedProjectsLikeSummary 是否已设置。 |
| keep_task_on_nearest_working_time_when_made_auto_scheduled | 获取或设置一个值，指示 KeepTaskOnNearestWorkingTimeWhenMadeAutoScheduled 是否已设置。 |
| keywords | 获取或设置 Keywords 的值。 |
| last_author | 获取或设置 LastAuthor 的值。 |
| last_printed | 获取或设置 LastPrinted 的值。 |
| last_saved | 获取或设置 LastSaved 的值。 |
| manager | 获取或设置 Manager 的值。 |
| microsoft_project_server_url | 获取或设置一个值，指示 MicrosoftProjectServerURL 是否已设置。 |
| minutes_per_day | 获取或设置 MinutesPerDay 的值。 |
| minutes_per_week | 获取或设置 MinutesPerWeek 的值。 |
| move_completed_ends_back | 获取或设置一个值，指示 MoveCompletedEndsBack 是否已设置。 |
| move_completed_ends_forward | 获取或设置一个值，指示 MoveCompletedEndsForward 是否已设置。 |
| move_remaining_starts_back | 获取或设置一个值，指示 MoveRemainingStartsBack 是否已设置。 |
| move_remaining_starts_forward | 获取或设置一个值，指示 MoveRemainingStartsForward 是否已设置。 |
| multiple_critical_paths | 获取或设置一个值，指示 MultipleCriticalPaths 是否已设置。 |
| name | 获取或设置 Name 的值。 |
| new_tasks_are_manual | 获取或设置一个值，指示 NewTasksAreManual 是否已设置。 |
| new_tasks_effort_driven | 获取或设置一个值，指示 NewTasksEffortDriven 是否已设置。 |
| new_tasks_estimated | 获取或设置一个值，指示 NewTasksEstimated 是否已设置。 |
| new_task_start_date | 获取或设置 NewTaskStartDate 的值。 |
| project_externally_edited | 获取或设置一个值，指示是否已设置 ProjectExternallyEdited。 |
| remove_file_properties | 获取或设置一个值，指示是否已设置 RemoveFileProperties。 |
| revision | 获取或设置 Revision 的值。 |
| save_version | 获取或设置 SaveVersion 的值。 |
| schedule_from_start | 获取或设置一个值，指示是否已设置 ScheduleFromStart。 |
| show_project_summary_task | 获取或设置一个值，指示是否已设置 ShowProjectSummaryTask。 |
| splits_in_progress_tasks | 获取或设置一个值，指示是否已设置 SplitsInProgressTasks。 |
| spread_actual_cost | 获取或设置一个值，指示是否已设置 SpreadActualCost。 |
| spread_percent_complete | 获取或设置一个值，指示是否已设置 SpreadPercentComplete。 |
| start_date | 获取或设置 StartDate 的值。 |
| status_date | 获取或设置 StatusDate 的值。 |
| subject | 获取或设置 Subject 的值。 |
| task_updates_resource | 获取或设置一个值，指示是否已设置 TaskUpdatesResource。 |
| template | 获取或设置 Template 的值。 |
| timescale_finish | 获取或设置 TimescaleFinish 的值。 |
| timescale_start | 获取或设置 TimescaleStart 的值。 |
| title | 获取或设置 Title 的值。 |
| uid | 获取或设置 Uid 的值。 |
| update_manually_scheduled_tasks_when_editing_links | 获取或设置一个值，指示是否已设置 UpdateManuallyScheduledTasksWhenEditingLinks。 |
| week_start_day | 获取或设置 WeekStartDay 的值。 |
| work_format | 获取或设置 WorkFormat 的值。 |
| guid | 获取或设置 Guid 的值。 |
| auto_calculate_assignment_costs | 获取或设置是否应使用任务的工作量和资源费率自动计算分配成本和剩余成本。 |
| default_view | 获取或设置项目的默认视图。 |
| vba_project | 获取 [vba_project](/tasks/python-net/aspose.tasks/project/) 类的实例。 |
| display_options | 获取 [ProjectDisplayOptions](/tasks/python-net/aspose.tasks/projectdisplayoptions/) 类的实例。 |
| calculation_mode | 获取或设置项目的计算模式。<br/>            可以是 [calculation_mode](/tasks/python-net/aspose.tasks/project/) 枚举的其中一个值。 |
| root_task | 获取任务树的根节点。 |
| task_links | 获取 [TaskLinkCollection](/tasks/python-net/aspose.tasks/tasklinkcollection/) 对象。 |
| calendars | 获取此 Project 实例的 [CalendarCollection](/tasks/python-net/aspose.tasks/calendarcollection/) 对象。 |
| 资源 | 获取 ResourceCollection 对象。 |
| 大纲代码 | 获取 OutlineCodeDefinitionCollection 对象。<br/>            与项目关联的大纲代码定义集合。 |
| 资源分配 | 获取 ResourceAssignmentCollection 对象。 |
| default_week_working_days | 获取 [WeekDayCollection](/tasks/python-net/aspose.tasks/weekdaycollection/) 类的实例，该实例表示项目默认工作周的工作日和工作时间的集合。 |
| 内置属性 | 获取项目的内置属性集合。 |
| 自定义属性 | 获取项目的自定义属性集合。 |
| extended_attributes | 获取 ExtendedAttributeDefinitionCollection 对象。<br/>            与项目关联的扩展属性（自定义字段）定义集合。 |
| 关键路径 | 获取一个集合，其中包含构成此项目关键路径的关键任务列表。 |
| task_filters | 获取所有基于任务的过滤器定义。 <br/>            TaskFilters 是 [Filter](/tasks/python-net/aspose.tasks/filter/) 对象的集合。 |
| resource_filters | 获取所有基于资源的过滤器定义。 <br/>            ResourceFilters 是 [Filter](/tasks/python-net/aspose.tasks/filter/) 对象的集合。 |
| views | 获取 [View](/tasks/python-net/aspose.tasks/view/) 对象的列表。 |
| tables | 获取 [Table](/tasks/python-net/aspose.tasks/table/) 对象的列表。 |
| task_groups | 获取所有基于任务的组定义。 <br/>            TaskGroups 是 [Group](/tasks/python-net/aspose.tasks/group/) 对象的集合。 |
| resource_groups | 获取所有基于资源的组定义。 <br/>            ResourceGroups 是 [Group](/tasks/python-net/aspose.tasks/group/) 对象的集合。 |
| WBS 代码定义 | 获取或设置项目的 WBS 代码定义。 |
| ole_objects | 获取一个集合，包含链接或嵌入到此项目文件的 [OleObject](/tasks/python-net/aspose.tasks/oleobject/) 类实例。 |
| Primavera 属性 | 获取一个对象，其中包含从 Primavera 文件读取的项目的 Primavera 特定属性。 |
| globalization_settings | 获取或设置项目的全球化（语言特定）设置。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| get_project_file_info(filename) | 从文件读取项目文件信息。 |
| get_project_file_info(stream) | 从流获取项目文件信息。 |
| recalculate() | 重新计算资源的开始和结束时间。 |
| recalculate(validate) | 重新安排所有项目任务的 ID、大纲级别、开始/结束日期，设置提前/延后日期，计算时差、工作量和成本字段，可选进行验证。 |
| save(filename, options) | 使用指定的保存选项将文档保存到文件。 |
| save(filename, format) | 将项目数据保存到文件。 |
| save(filename) | 使用指定的保存选项将文档保存到文件。 |
| save(stream, options) | 使用指定的保存选项将项目保存到流。 |
| save(stream, format) | 将项目数据保存到流。 |
| save_report(stream) | 将项目概览报告保存到流。 |
| save_report(file_name) | 将项目概览报告保存为 PDF 文件。 |
| save_report(stream, report_type) | 将指定类型的项目报告保存到指定的流中。 |
| save_report(file_name, report_type) | 将指定类型的项目报告以 PDF 格式保存到指定的文件路径。 |
| save_as_template(file_name, options) | 将项目保存为模板。 |
| save_as_template(file_name) | 将项目保存为模板。 |
| save_as_template(stream) | 将项目保存为模板到指定的流。 |
| save_as_template(stream, options) | 将项目保存为模板到指定的流。 |
| get_page_count(save_options) | 返回使用给定的 [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/) 渲染项目的页数。 |
| get_page_count() | 返回使用给定的 [SaveOptions](/tasks/python-net/aspose.tasks.saving/saveoptions/) 渲染项目的页数。 |
| get_page_count(scale) | 返回使用给定的 [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/) 渲染项目的页数。 |
| get_page_count(format) | 返回使用默认的 [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)(天) 和给定的 [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 渲染项目的页数 |
| get_page_count(format, scale) | 返回使用给定的 [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/) 和 [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 渲染项目的页数。 |
| get_page_count(page_size, scale, start_date, end_date) | 返回使用给定的 [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)、[PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 和日期范围渲染项目的页数。 |
| get_page_count(page_size, scale) | 返回使用给定的 [Timescale](/tasks/python-net/aspose.tasks.visualization/timescale/)、[PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) 和日期范围渲染项目的页数。 |
| copy_to(another) | 将项目的主要数据和属性复制到另一个项目。 |
| copy_to(another, options) | 将项目的主要数据和属性复制到另一个项目。 |
| print() | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机并使用默认打印机设置。 |
| print(options) | 使用标准（无用户界面）打印控制器，将项目打印到默认打印机，使用默认打印机设置和自定义保存选项。 |
| print(printer_name) | 使用标准（无用户界面）打印控制器，将项目打印到指定的打印机并使用默认打印机设置。 |
| print(printer_settings) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| print(printer_settings, document_name) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置打印项目。 |
| print(printer_settings, options) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置和自定义保存选项打印项目。 |
| print(printer_settings, options, document_name) | 使用标准（无用户界面）打印控制器，根据指定的打印机设置、自定义保存选项和指定的文档名称打印项目。 |
| set_baseline(baseline_type) | 设置基准保存时间。 |
| set_baseline(baseline_type, task_collection) |  |
| update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only) | 将整个项目中截至指定日期的所有工作标记为完成。 |
| update_project_work_as_complete(complete_through, set_zero_or_hundred_percent_complete_only, task_collection) |  |
| reschedule_uncompleted_work_to_start_after(after) | 将未完成的项目工作重新安排为在指定日期之后开始。 |
| reschedule_uncompleted_work_to_start_after(after, task_collection) |  |
| renumber_wbs_code() | 重新编号所有任务的 WBS 代码。 |
| renumber_wbs_code(task_ids) |  |
| get_duration(val) | 获取具有指定单位数和默认持续时间格式的 [Duration](/tasks/python-net/aspose.tasks/duration/) 对象，默认格式在项目设置 [None](/tasks/python-net/aspose.tasks/prj/) 中定义。 |
| get_duration(val, time_unit) | 获取具有指定数量的 [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) 单位的 [Duration](/tasks/python-net/aspose.tasks/duration/) 对象。 |
| get_duration(time_span, time_unit) | 获取具有指定日期时间值和指定 [TimeUnitType](/tasks/python-net/aspose.tasks/timeunittype/) 值的 [Duration](/tasks/python-net/aspose.tasks/duration/) 对象。 |
| select_all_child_tasks() | 递归收集根任务的所有子任务。 |
| enumerate_all_child_tasks() | 递归枚举项目的所有任务，包括根任务。 |
| get_predecessors(task) | 返回指定任务的前置任务链接集合。 |
| recalculate_resource_start_finish() | 重新计算资源的开始和结束时间。 |
| recalculate_resource_fields() | 重新计算资源的 Id、开始和结束。 |
| remove_invalid_resource_assignments() | 从项目资源分配列表中删除无效的资源分配。 |
| get_baseline_save_time(baseline_number) | 返回基准保存时间。 |
| set_baseline_save_time(baseline_number, value) | 设置基准保存时间。 |
| get_work(val) | 获取具有指定浮点值和默认工作格式的 [Duration](/tasks/python-net/aspose.tasks/duration/) 对象。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

