---
title: FilterCriteria
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 350
url: /python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Defines the criteria that tasks or resources must meet to be displayed in MSP view.

The FilterCriteria type exposes the following members:
## Constructors
| Name | Description |
| :- | :- |
|FilterCriteria()|Initializes a new instance of the FilterCriteria class|
## Properties
| Name | Description |
| :- | :- |
|operation|Gets or sets the criterion established with FieldName, Test, and Value relates to other criteria in the filter.|
|field|Gets or sets a [field](/tasks/python-net/aspose.tasks/filtercriteria/) to change.|
|test|Gets or sets the type of comparison made between FieldName and Value that acts as selection criteria for the filter.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/)|
|values|Gets the object values to compare with the value of the field specified with FieldName.|
|criteria_rows|Gets the list of child [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) rows.<br/>            If the filter contains more than one criterion row then the effect of an And operator is that the criteria for both rows must be met for the task or resource to be displayed as a result of this filter.<br/>            The effect of an Or operator is that the criteria for one or the other row must be met.|
## Methods
| Name | Description |
| :- | :- |
|is_field_value()|Gets whether the right-hand value of FilterCriteria is a field reference, not a constant value.|
|set_value_field(value)|Sets the field whose value will be compared with the value of the field specified by FieldName.|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

