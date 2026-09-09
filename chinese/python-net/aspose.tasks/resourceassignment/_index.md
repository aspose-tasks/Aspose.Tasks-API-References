---
title: "ResourceAssignment"
second_title: "适用于 Python via .NET 的 Aspose.Tasks API 参考"
description: 
type: docs
weight: 980
url: /zh/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

表示项目中的资源分配。

该 ResourceAssignment 类型公开以下成员：
## 属性
| 名称 | 描述 |
| :- | :- |
| uid | 获取或设置 Uid 的值。 |
| percent_work_complete | 获取或设置 PercentWorkComplete 的值。 |
| actual_cost | 获取或设置 ActualCost 的值. |
| actual_finish | 获取或设置 ActualFinish 的值。 |
| actual_overtime_cost | 获取或设置 ActualOvertimeCost 的值. |
| actual_start | 获取或设置 ActualStart 的值。 |
| actual_work | 获取或设置 ActualWork 的值. |
| acwp | 获取或设置 ACWP 的值. |
| confirmed | 获取或设置一个值，指示 Confirmed 是否已设置。 |
| cost | 获取或设置 Cost 的值。 |
| cost_rate_table_type | 获取或设置 CostRateTableType 的值。 |
| cost_variance | 获取或设置 CostVariance 的值。 |
| cv | 获取或设置 CV 的值。 |
| delay | 获取或设置 Delay 的值。 |
| finish | 获取或设置 Finish 的值。 |
| finish_variance | 获取或设置 FinishVariance 的值。 |
| hyperlink | 获取或设置 Hyperlink 的值。 |
| hyperlink_address | 获取或设置 HyperlinkAddress 的值。 |
| hyperlink_sub_address | 获取或设置 HyperlinkSubAddress 的值。 |
| work_variance | 获取或设置 WorkVariance 的值。 |
| has_fixed_rate_units | 获取或设置一个值，指示 HasFixedRateUnits 是否已设置。 |
| fixed_material | 获取或设置一个值，指示 FixedMaterial 是否已设置。 |
| leveling_delay | 获取或设置 LevelingDelay 的值。 |
| linked_fields | 获取或设置一个值，指示 LinkedFields 是否已设置。 |
| milestone | 获取或设置一个值，指示 Milestone 是否已设置。 |
| notes_text | 获取或设置从 RTF 数据中提取的 notes 的纯文本。 |
| notes_rtf | 获取或设置 RTF 格式的文本备注。 |
| overallocated | 获取或设置一个值，指示 Overallocated 是否已设置。 |
| overtime_cost | 获取或设置 OvertimeCost 的值。 |
| overtime_work | 获取或设置 OvertimeWork 的值。 |
| peak_units | 获取或设置 PeakUnits 的值。 |
| regular_work | 获取或设置 RegularWork 的值。 |
| remaining_cost | 获取或设置 RemainingCost 的值。 |
| remaining_overtime_cost | 获取或设置 RemainingOvertimeCost 的值。 |
| remaining_overtime_work | 获取或设置 RemainingOvertimeWork 的值。 |
| remaining_work | 获取或设置 RemainingWork 的值。 |
| response_pending | 获取或设置一个值，指示是否已设置 ResponsePending。 |
| 开始 | 获取或设置 Start 的值。 |
| stop | 获取或设置 Stop 的值。 |
| resume | 获取或设置 Resume 的值。 |
| start_variance | 获取或设置 StartVariance 的值。 |
| summary | 获取或设置一个值，指示是否已设置 Summary。 |
| sv | 获取或设置 SV 的值。 |
| units | 获取或设置 Units 的值。 |
| update_needed | 获取或设置一个值，指示是否已设置 UpdateNeeded。 |
| vac | 获取或设置 VAC 的值。 |
| work | 获取或设置 Work 的值。 |
| work_contour | 获取或设置 WorkContour 的值。 |
| bcws | 获取或设置 BCWS 的值。 |
| bcwp | 获取或设置 BCWP 的值。 |
| booking_type | 获取或设置 BookingType 的值。 |
| actual_work_protected | 获取或设置 ActualWorkProtected 的值. |
| actual_overtime_work_protected | 获取或设置 ActualOvertimeWorkProtected 的值. |
| actual_overtime_work | 获取或设置 ActualOvertimeWork 的值. |
| created | 获取或设置 Created 的值。 |
| assignment_owner | 获取或设置 AssignmentOwner 的值. |
| assignment_owner_guid | 获取或设置 AssignmentOwnerGuid 的值. |
| budget_cost | 获取或设置 BudgetCost 的值。 |
| budget_work | 获取或设置 BudgetWork 的值。 |
| rate_scale | 获取或设置 RateScale 的值。 |
| task | 已分配资源的任务。 |
| resource | 已分配给任务的资源。 |
| guid | 获取或设置此分配的唯一标识符。 |
| parent_project | 获取此分配的父项目。 |
| baselines | 获取 AssignmentBaselineCollection 对象。<br/>            与分配关联的基线值集合。 |
| extended_attributes | 获取或设置此对象的 ExtendedAttributeCollection 类的实例。 |
| timephased_data | 获取或设置 [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) 类的实例，该实例包含 [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) 类的元素。 |
## Methods
| 名称 | 描述 |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | 返回 [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) 类的实例，该实例在指定的 [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) 的给定开始和结束日期范围内包含 [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) 类的实例。 |
| get_timephased_data(start, end) | 返回 [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) 类的实例，该实例在指定的 [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) 的给定开始和结束日期范围内包含 [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) 类的实例。 |
| get_timephased_work(start, end, timephased_data_type) | 获取指定日期时间区间的分阶段工作量。 |
| get_timephased_work(start, end) | 获取指定日期时间区间的分阶段工作量。 |
| delete() | 从项目分配集合中删除资源分配。 |
| equals(other) | 返回一个值，指示此实例是否等于指定的 [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/) 类的实例。 |
| timephased_data_from_task_duration(calendar) | 根据任务持续时间和计划开始日期生成分阶段数据列表。 |
| make_t_ps(start, time, calendar, list, is_working, type) | 生成分阶段数据列表。 |
| split_task(start, finish, calendar) | 将任务拆分为两部分。 |
| set_material_resource_units(units, rate_scale_type) | 为具有可变材料消耗的材料资源分配设置单位。<br/>            可变材料消耗意味着随着分配持续时间的变化，使用的材料数量按比例变化。 |

### 另见

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

