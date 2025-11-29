---
title: Resource
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 970
url: /python-net/aspose.tasks/resource/
---

## Resource class

Represents a resource in a project.

The Resource type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|accrue_at|Gets or sets a value of AccrueAt.|
|active_directory_guid|Gets or sets a value of ActiveDirectoryGuid.|
|actual_cost|Gets or sets a value of ActualCost.|
|actual_overtime_cost|Gets or sets a value of ActualOvertimeCost.|
|actual_overtime_work|Gets or sets a value of ActualOvertimeWork.|
|actual_overtime_work_protected|Gets or sets a value of ActualOvertimeWorkProtected.|
|actual_work|Gets or sets a value of ActualWork.|
|actual_work_protected|Gets or sets a value of ActualWorkProtected.|
|acwp|Gets or sets a value of ACWP.|
|assignment_owner|Gets or sets a value of AssignmentOwner.|
|assignment_owner_guid|Gets or sets a value of AssignmentOwnerGuid.|
|available_from|Gets or sets a value of AvailableFrom.|
|available_to|Gets or sets a value of AvailableTo.|
|bcwp|Gets or sets a value of BCWP.|
|bcws|Gets or sets a value of BCWS.|
|booking_type|Gets or sets a value of BookingType.|
|budget_cost|Gets or sets a value of BudgetCost.|
|budget_work|Gets or sets a value of BudgetWork.|
|calendar|Gets or sets a value of Calendar.|
|can_level|Gets or sets a value indicating whether CanLevel is set or not.|
|code|Gets or sets a value of Code.|
|cost|Gets or sets a value of Cost.|
|cost_center|Gets or sets a value of CostCenter.|
|cost_per_use|Gets or sets a value of CostPerUse.|
|cost_variance|Gets or sets a value of CostVariance.|
|created|Gets or sets a value of Created.|
|cv|Gets or sets a value of CV.|
|e_mail_address|Gets or sets a value of EMailAddress.|
|finish|Gets or sets a value of Finish.|
|group|Gets or sets a value of Group.|
|guid|Gets or sets a value of Guid.|
|hyperlink|Gets or sets the title or explanatory text of a hyperlink associated with a resource.|
|hyperlink_address|Gets or sets the address for a hyperlink associated with a resource.|
|hyperlink_sub_address|Gets or sets the specific location in a document in a hyperlink associated with a resource.|
|id|Gets or sets a value of Id.|
|inactive|Gets or sets a value indicating whether Inactive is set or not.|
|initials|Gets or sets a value of Initials.|
|is_budget|Gets or sets a value indicating whether IsBudget is set or not.|
|is_cost_resource|Gets or sets a value indicating whether IsCostResource is set or not.|
|is_enterprise|Gets or sets a value indicating whether IsEnterprise is set or not.|
|is_generic|Gets or sets a value indicating whether IsGeneric is set or not.|
|is_null|Gets or sets a value indicating whether IsNull is set or not.|
|is_team_assignment_pool|Gets or sets a value indicating whether IsTeamAssignmentPool is set or not.|
|material_label|Gets or sets a value of MaterialLabel.|
|max_units|Gets or sets a value of MaxUnits.|
|name|Gets or sets a value of Name.|
|notes_rtf|Gets or sets a value of NotesRTF.|
|notes_text|Gets or sets a value of NotesText.|
|overallocated|Gets or sets a value indicating whether Overallocated is set or not.|
|overtime_cost|Gets or sets a value of OvertimeCost.|
|overtime_rate|Gets or sets a value of OvertimeRate.|
|overtime_rate_format|Gets or sets a value of OvertimeRateFormat.|
|overtime_work|Gets or sets a value of OvertimeWork.|
|peak_units|Gets or sets a value of PeakUnits.|
|percent_work_complete|Gets or sets a value of PercentWorkComplete.|
|phonetics|Gets or sets a value of Phonetics.|
|regular_work|Gets or sets a value of RegularWork.|
|remaining_cost|Gets or sets a value of RemainingCost.|
|remaining_overtime_cost|Gets or sets a value of RemainingOvertimeCost.|
|remaining_overtime_work|Gets or sets a value of RemainingOvertimeWork.|
|remaining_work|Gets or sets a value of RemainingWork.|
|standard_rate|Gets or sets a value of StandardRate.|
|standard_rate_format|Gets or sets a value of StandardRateFormat.|
|start|Gets or sets a value of Start.|
|sv|Gets or sets a value of SV.|
|type|Gets or sets a value of Type.|
|uid|Gets or sets a value of Uid.|
|windows_user_account|Gets or sets a value of WindowsUserAccount.|
|work|Gets or sets a value of Work.|
|workgroup|Gets or sets a value of Workgroup.|
|work_variance|Gets or sets a value of WorkVariance.|
|parent_project|Gets parent project for this container.|
|extended_attributes|Gets the values of an extended attribute.|
|baselines|Gets a BaselineCollection instance for this object.<br/>            The baseline values for a resource.|
|outline_code|Gets an OutlineCodeCollection object.<br/>            The value of an outline code.|
|availability_periods|Gets a the instance of the [AvailabilityPeriodCollection](/tasks/python-net/aspose.tasks/availabilityperiodcollection/) class.<br/>            The collection of periods during which a resource is available.|
|rates|Gets a the instance of the [RateCollection](/tasks/python-net/aspose.tasks/ratecollection/) class for this object.<br/>            The collection of periods and rates associated with each one.|
|assignments|Gets a collection of resource assignments for this object.|
|timephased_data|Gets or sets an instance of [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class for this object.|
|is_root|Gets the flag indicating whether resource is a root resource.<br/>            Root resource is a special resource which is intended to support internals of<br/>            MS Project's formats and is not intended to be used directly from the user's code.|
## Methods
| Name | Description |
| :- | :- |
|get_timephased_data(start, end, timephased_type)|Returns an instance of the [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class for this object with the [timephased_data](/tasks/python-net/aspose.tasks/resource/) values within given start and end dates of specified [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/).|
|get_timephased_data(start, end)|Returns an instance of the [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) class for this object with the [timephased_data](/tasks/python-net/aspose.tasks/resource/) values within given start and end dates of specified [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/).|
|equals(other)|Returns a value indicating whether this instance is equal to a specified instance of the [Resource](/tasks/python-net/aspose.tasks/resource/) class.|
|delete()|Deletes a resource and its assignments from project.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

