---
title: ResourceAssignment
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 980
url: /python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Represents a resource assignment in a project.

The ResourceAssignment type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|uid|Gets or sets a value of Uid.|
|percent_work_complete|Gets or sets a value of PercentWorkComplete.|
|actual_cost|Gets or sets a value of ActualCost.|
|actual_finish|Gets or sets a value of ActualFinish.|
|actual_overtime_cost|Gets or sets a value of ActualOvertimeCost.|
|actual_start|Gets or sets a value of ActualStart.|
|actual_work|Gets or sets a value of ActualWork.|
|acwp|Gets or sets a value of ACWP.|
|confirmed|Gets or sets a value indicating whether Confirmed is set or not.|
|cost|Gets or sets a value of Cost.|
|cost_rate_table_type|Gets or sets a value of CostRateTableType.|
|cost_variance|Gets or sets a value of CostVariance.|
|cv|Gets or sets a value of CV.|
|delay|Gets or sets a value of Delay.|
|finish|Gets or sets a value of Finish.|
|finish_variance|Gets or sets a value of FinishVariance.|
|hyperlink|Gets or sets a value of Hyperlink.|
|hyperlink_address|Gets or sets a value of HyperlinkAddress.|
|hyperlink_sub_address|Gets or sets a value of HyperlinkSubAddress.|
|work_variance|Gets or sets a value of WorkVariance.|
|has_fixed_rate_units|Gets or sets a value indicating whether HasFixedRateUnits is set or not.|
|fixed_material|Gets or sets a value indicating whether FixedMaterial is set or not.|
|leveling_delay|Gets or sets a value of LevelingDelay.|
|linked_fields|Gets or sets a value indicating whether LinkedFields is set or not.|
|milestone|Gets or sets a value indicating whether Milestone is set or not.|
|notes_text|Gets or sets notes' plain text extracted from RTF data.|
|notes_rtf|Gets or sets the text notes in RTF format.|
|overallocated|Gets or sets a value indicating whether Overallocated is set or not.|
|overtime_cost|Gets or sets a value of OvertimeCost.|
|overtime_work|Gets or sets a value of OvertimeWork.|
|peak_units|Gets or sets a value of PeakUnits.|
|regular_work|Gets or sets a value of RegularWork.|
|remaining_cost|Gets or sets a value of RemainingCost.|
|remaining_overtime_cost|Gets or sets a value of RemainingOvertimeCost.|
|remaining_overtime_work|Gets or sets a value of RemainingOvertimeWork.|
|remaining_work|Gets or sets a value of RemainingWork.|
|response_pending|Gets or sets a value indicating whether ResponsePending is set or not.|
|start|Gets or sets a value of Start.|
|stop|Gets or sets a value of Stop.|
|resume|Gets or sets a value of Resume.|
|start_variance|Gets or sets a value of StartVariance.|
|summary|Gets or sets a value indicating whether Summary is set or not.|
|sv|Gets or sets a value of SV.|
|units|Gets or sets a value of Units.|
|update_needed|Gets or sets a value indicating whether UpdateNeeded is set or not.|
|vac|Gets or sets a value of VAC.|
|work|Gets or sets a value of Work.|
|work_contour|Gets or sets a value of WorkContour.|
|bcws|Gets or sets a value of BCWS.|
|bcwp|Gets or sets a value of BCWP.|
|booking_type|Gets or sets a value of BookingType.|
|actual_work_protected|Gets or sets a value of ActualWorkProtected.|
|actual_overtime_work_protected|Gets or sets a value of ActualOvertimeWorkProtected.|
|actual_overtime_work|Gets or sets a value of ActualOvertimeWork.|
|created|Gets or sets a value of Created.|
|assignment_owner|Gets or sets a value of AssignmentOwner.|
|assignment_owner_guid|Gets or sets a value of AssignmentOwnerGuid.|
|budget_cost|Gets or sets a value of BudgetCost.|
|budget_work|Gets or sets a value of BudgetWork.|
|rate_scale|Gets or sets a value of RateScale.|
|task|The task to which a resource is assigned.|
|resource|The resource assigned to a task.|
|guid|Gets or sets unique identifier for this assignment.|
|parent_project|Gets parent project for this assignment.|
|baselines|Gets AssignmentBaselineCollection object.<br/>            The collection of baseline values associated with an assignment.|
|extended_attributes|Gets or sets an instance of the ExtendedAttributeCollection class for this object.|
|timephased_data|Gets or sets the instance of [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class containing elements of [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) class.|
## Methods
| Name | Description |
| :- | :- |
|get_timephased_data(start, end, timephased_type)|Returns the instance [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class containing instances of [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) class within given start and end dates of specified [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/).|
|get_timephased_data(start, end)|Returns the instance [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class containing instances of [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) class within given start and end dates of specified [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/).|
|get_timephased_work(start, end, timephased_data_type)|Gets amount of timephased work for the specified date time interval.|
|get_timephased_work(start, end)|Gets amount of timephased work for the specified date time interval.|
|delete()|Deletes resource assignment from project assignments collection.|
|equals(other)|Returns a value indicating whether this instance is equal to a specified instance of the [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/) class.|
|timephased_data_from_task_duration(calendar)|Generates list of time phased data based on the task duration and the scheduled start date.|
|make_t_ps(start, time, calendar, list, is_working, type)|Generates a list of time phased data.|
|split_task(start, finish, calendar)|Splits task into two parts.|
|set_material_resource_units(units, rate_scale_type)|Sets units for assignment of a material resource with variable material consumption.<br/>            The variable material consumption means that as the assignment duration changes, the quantity of materials used changes proportionally.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

