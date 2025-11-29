---
title: PrimaveraProjectProperties
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 760
url: /python-net/aspose.tasks/primaveraprojectproperties/
---

## PrimaveraProjectProperties class

Represents Primavera-specific properties for a project read from Primavera files (XER of P6XML).

The PrimaveraProjectProperties type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|relationship_lag_calendar|Gets an options which defines which calendar to use for scheduling Relationship Lag in Primavera projects|
|use_expected_finish_dates|Gets a flag which defines whether activity finish dates should be scheduled as the expected finish dates.|
|make_open_ended_activities_critical|Gets a flag which defines whether activities should me marked as critical when scheduling the project.|
|ignore_other_project_relationships|Gets a flag which defines whether to ignore activity relationships between projects.|
|current_baseline_project_id|Gets Id of the current baseline project.<br/>            Is applicable to projects read from Primavera XML files containing exported baselines.|
|baseline_projects|Gets array of baseline projects of current project.<br/>            Is applicable to projects read from Primavera XML files containing exported baselines.|
|critical_activities_defining_method|Gets the method for defining critical activities: Longest Path or Total Float approach.|
|critical_total_float_limit|Gets the threshold value used to define critical activities if TotalFloat method is used.|
|short_name|Gets project's short name (Project ID).|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

