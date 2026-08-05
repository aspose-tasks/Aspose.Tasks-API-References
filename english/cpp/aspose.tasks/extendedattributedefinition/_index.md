---
title: "Aspose::Tasks::ExtendedAttributeDefinition class"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks for C++"
description: "Represents an extended attribute definition associated with a project."
type: docs
weight: 10
url: /cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Represents an extended attribute definition associated with a project.

## Methods

| Name | Description |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Adds a value to the internal lookup list. This is a preferable way for manipulations with the ValueList . |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Creates a new extended attribute with the field ID which equals to this object's field ID value. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Resources only. You are required to specify customFieldType , fieldId and alias when call this method. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Tasks::CalculationType::Lookup and can be used in Tasks only. You are required to specify customFieldType , fieldId and alias when call this method. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Resource only. You are required to specify customFieldType , fieldId and alias when call this method. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has CalculationType equals to Tasks::CalculationType::None and can be used in Tasks only. You are required to specify customFieldType , fieldId and alias when calling this method. |
| [Equals](./equals/) | Returns a flag indicating whether this instance is equal to the specified object. |
| [get_Alias](./get_alias/) | Gets the alias of a custom field. |
| [get_AppendNewValues](./get_appendnewvalues/) | Gets a value indicating whether new values added to a project are automatically added to the list. |
| [get_AutoRollDown](./get_autorolldown/) | Gets a value indicating whether an automatic roll down to assignments is enabled. |
| [get_CalculationType](./get_calculationtype/) | Gets the type of calculation of the custom attribute's value. |
| [get_CfType](./get_cftype/) | Gets the type of a custom field. |
| [get_Default](./get_default/) | Gets the default value in the list. |
| [get_DefaultGuid](./get_defaultguid/) | Gets the Guid of the default lookup table entry. |
| [get_ElementType](./get_elementtype/) | Gets the extended attribute is associated with a task, a resource or an assignment. |
| [get_FieldId](./get_fieldid/) | Gets corresponds to the project id of a custom field. Use string representation of a constant from Aspose::Tasks::ExtendedAttributeTask class to specify FieldId property. |
| [get_FieldName](./get_fieldname/) | Gets the name of a custom field. |
| [get_Formula](./get_formula/) | Gets the formula that Microsoft Project uses to populate a custom task field. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Gets a graphical indicators info associated with the extended attribute. Applicable to MPP format. |
| [get_Guid](./get_guid/) | Gets the Guid of a custom field. |
| [get_LookupUid](./get_lookupuid/) | Gets a Guid of the lookup table associated with a custom field. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Gets the maximum number of values you can set in a pick list. |
| [get_ParentProject](./get_parentproject/) | Gets the parent project for the ExtendedAttributeDefinition instance. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Gets the phonetic pronunciation of the alias of a custom field. |
| [get_RestrictValues](./get_restrictvalues/) | Gets a value indicating whether the custom field values are restricted to values in the ValueList . |
| [get_RollupType](./get_rolluptype/) | Gets the way rollups are calculated. |
| [get_SecondaryGuid](./get_secondaryguid/) | Gets the secondary guid of extended attribute. |
| [get_SecondaryPid](./get_secondarypid/) | Gets the secondary PID of a custom field. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Gets the type of calculation of the custom attribute's value for summary rows. |
| [get_UserDef](./get_userdef/) | Gets a value indicating whether a custom field is user defined. |
| [get_ValueList](./get_valuelist/) | Gets the List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Gets the way value lists are sorted. Values are: 0=Descending, 1=Ascending. |
| [GetHashCode](./gethashcode/) | Returns a hash code for the instance of the ExtendedAttributeDefinition class. |
| [RemoveLookupValue](./removelookupvalue/) | Removes a value from the internal lookup list. This is a preferable way for manipulations with the ValueList . |
| [set_Alias](./set_alias/) | Sets the alias of a custom field. |
| [set_AppendNewValues](./set_appendnewvalues/) | Sets a value indicating whether new values added to a project are automatically added to the list. |
| [set_AutoRollDown](./set_autorolldown/) | Sets a value indicating whether an automatic roll down to assignments is enabled. |
| [set_CalculationType](./set_calculationtype/) | Sets the type of calculation of the custom attribute's value. |
| [set_Default](./set_default/) | Sets the default value in the list. |
| [set_DefaultGuid](./set_defaultguid/) | Sets the Guid of the default lookup table entry. |
| [set_ElementType](./set_elementtype/) | Sets the extended attribute is associated with a task, a resource or an assignment. |
| [set_FieldId](./set_fieldid/) | Sets corresponds to the project id of a custom field. Use string representation of a constant from Aspose::Tasks::ExtendedAttributeTask class to specify FieldId property. |
| [set_Formula](./set_formula/) | Sets the formula that Microsoft Project uses to populate a custom task field. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Sets a graphical indicators info associated with the extended attribute. Applicable to MPP format. |
| [set_Guid](./set_guid/) | Sets the Guid of a custom field. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Sets the maximum number of values you can set in a pick list. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Sets the phonetic pronunciation of the alias of a custom field. |
| [set_RestrictValues](./set_restrictvalues/) | Sets a value indicating whether the custom field values are restricted to values in the ValueList . |
| [set_RollupType](./set_rolluptype/) | Sets the way rollups are calculated. |
| [set_SecondaryGuid](./set_secondaryguid/) | Sets the secondary guid of extended attribute. |
| [set_SecondaryPid](./set_secondarypid/) | Sets the secondary PID of a custom field. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Sets the type of calculation of the custom attribute's value for summary rows. |
| [set_UserDef](./set_userdef/) | Sets a value indicating whether a custom field is user defined. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Sets the way value lists are sorted. Values are: 0=Descending, 1=Ascending. |

