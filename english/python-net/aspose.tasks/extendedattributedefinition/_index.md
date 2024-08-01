---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks for Python via .NET API Reference
description: 
type: docs
weight: 310
url: /python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Represents an extended attribute definition associated with a project.

The ExtendedAttributeDefinition type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|field_id|Gets or sets corresponds to the project id of a custom field.<br/>            Use string representation of a constant from|
|field_name|Gets the name of a custom field.|
|cf_type|Gets the type of a custom field.|
|guid|Gets or sets the Guid of a custom field.|
|element_type|Gets or sets the extended attribute is associated<br/>            with a task, a resource or an assignment.|
|max_multi_values|Gets or sets the maximum number of values you can set in a pick list.|
|user_def|Gets or sets a value indicating whether a custom field is user defined.|
|alias|Gets or sets the alias of a custom field.|
|secondary_pid|Gets or sets the secondary PID of a custom field.|
|auto_roll_down|Gets or sets a value indicating whether an automatic roll down to assignments is enabled.|
|default_guid|Gets or sets the Guid of the default lookup table entry.|
|lookup_uid|Gets a Guid of the lookup table associated with a custom field.|
|phonetics_alias|Gets or sets the phonetic pronunciation of the alias of a custom field.|
|rollup_type|Gets or sets the way rollups are calculated.|
|calculation_type|Gets or sets the type of calculation of the custom attribute's value.|
|summary_rows_calculation_type|Gets or sets the type of calculation of the custom attribute's value for summary rows.|
|formula|Gets or sets the formula that Microsoft Project uses to populate a custom task field.|
|restrict_values|Gets or sets a value indicating whether the custom field values are restricted to values in the|
|valuelist_sort_order|Gets or sets the way value lists are sorted. Values are: 0=Descending, 1=Ascending.|
|append_new_values|Gets or sets a value indicating whether new values added to a project are automatically added to the list.|
|default|Gets or sets the default value in the list.|
|value_list|Gets the List<Value> ValueList.|
|secondary_guid|Gets or sets the secondary guid of extended attribute.|
|parent_project|Gets the parent project for the|
## Methods
| Name | Description |
| :- | :- |
|create_extended_attribute()|Creates a new extended attribute with the field ID which equals to this object's field ID value.|
|create_extended_attribute(text_value)|Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified text value.|
|create_extended_attribute(numeric_value)|Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified numeric value.|
|create_extended_attribute(date_time_value)|Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified date value.|
|create_extended_attribute(duration_value)|Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value.|
|create_extended_attribute(flag_value)|Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value.|
|create_extended_attribute(lookup_value)|Creates new extended attribute linked with specified|
|create_task_definition(custom_field_type, field_id, alias)|Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None".<br/>            It has|
|create_task_definition(field_id, alias)|Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None".<br/>            It has|
|create_resource_definition(custom_field_type, field_id, alias)|Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None".<br/>            It has|
|create_resource_definition(field_id, alias)|Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None".<br/>            It has|
|create_lookup_task_definition(field_id, alias)|Factory method which creates an extended attribute definition with lookup.<br/>            It has|
|create_lookup_task_definition(custom_field_type, field_id, alias)|Factory method which creates an extended attribute definition with lookup.<br/>            It has|
|create_lookup_resource_definition(field_id, alias)|Factory method which creates an extended attribute definition with lookup.<br/>            It has|
|create_lookup_resource_definition(custom_field_type, field_id, alias)|Factory method which creates an extended attribute definition with lookup.<br/>            It has|
|add_lookup_value(value)|Adds a value to the internal lookup list. This is a preferable way for manipulations with the|
|remove_lookup_value(value)|Removes a value from the internal lookup list. This is a preferable way for manipulations with the|

### See Also

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

