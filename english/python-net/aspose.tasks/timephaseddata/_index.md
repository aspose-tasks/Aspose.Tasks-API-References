---
title: TimephasedData
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 1270
url: /python-net/aspose.tasks/timephaseddata/
---

## TimephasedData class

Represents a time phased data.

The TimephasedData type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|TimephasedData()|Initializes a new instance of the [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) class.|
## Properties
| Name | Description |
| :- | :- |
|value_to_units|Gets float instance which represents string value of this object for unit-based time phased data.|
|uid|Gets or sets the unique identifier of a time phased data|
|start|Gets or sets the start date of a time phased data period.|
|finish|Gets or sets the finish date of a time phased data period.|
|unit|Gets or sets the time unit of a time phased data period.|
|timephased_data_type|Gets or sets the type of a time phased data.|
|value|Gets or sets the value per unit of time for a time phased data period.|
|value_to_duration|Gets datatime instance which represents string value of this object.|
|value_to_cost|Gets float instance which represents string value of this object.|
## Methods
| Name | Description |
| :- | :- |
|create_cost_timephased(uid, start, finish, value, time_unit, type)|  |
|create_cost_timephased(uid, start, finish, value, type)|  |
|create_work_timephased(uid, start, finish, value, time_unit, type)|Creates and initializes a new instance of the [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) class for work-based time phased data.|
|create_unit_timephased(uid, start, finish, units, type)|Creates and initializes a new instance of the [TimephasedData](/tasks/python-net/aspose.tasks/timephaseddata/) class for unit-based time phased data of an assignment of a material resource.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

