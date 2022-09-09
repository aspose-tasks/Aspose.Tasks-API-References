---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API Reference
description: Represents an extended attribute definition associated with a project.
type: docs
weight: 530
url: /net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Represents an extended attribute definition associated with a project.

```csharp
public class ExtendedAttributeDefinition
```

## Properties

| Name | Description |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Gets or sets the alias of a custom field. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Gets or sets a value indicating whether new values added to a project are automatically added to the list. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Gets or sets a value indicating whether an automatic roll down to assignments is enabled. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Gets or sets the type of calculation of the custom attribute's value. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Gets the type of a custom field. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Gets or sets the default value in the list. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Gets or sets the Guid of the default lookup table entry. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Gets or sets the extended attribute is associated with a task, a resource or an assignment. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Gets or sets corresponds to the project id of a custom field. Use string representation of a constant from [`ExtendedAttributeTask`](../extendedattributetask) class to specify [`FieldId`](./fieldid) property. |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Gets the name of a custom field. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Gets or sets the formula that Microsoft Project uses to populate a custom task field. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Gets or sets the Guid of a custom field. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Gets a Guid of the lookup table associated with a custom field. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Gets or sets the maximum number of values you can set in a pick list. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Gets the parent project for the [`ExtendedAttributeDefinition`](../extendedattributedefinition) instance. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Gets or sets the phonetic pronunciation of the alias of a custom field. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Gets or sets a value indicating whether the custom field values are restricted to values in the [`ValueList`](./valuelist). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Gets or sets the way rollups are calculated. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Gets or sets the secondary guid of extended attribute. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Gets or sets the secondary PID of a custom field. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Gets or sets the type of calculation of the custom attribute's value for summary rows. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Gets or sets a value indicating whether a custom field is user defined. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Gets the List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Gets or sets the way value lists are sorted. Values are: 0=Descending, 1=Ascending. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Resources only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Resources only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Tasks only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Tasks only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Resource only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Resource only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Tasks only. You are required to specify *fieldId* and *alias* when calling this method. The field type is inferred from field id. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Tasks only. You are required to specify *customFieldType*, *fieldId* and *alias* when calling this method. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Adds a value to the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](./valuelist). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Creates a new extended attribute with the field ID which equals to this object's field ID value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified date value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified numeric value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified text value. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Creates new extended attribute linked with specified [`Value`](../value) item. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Returns a flag indicating whether this instance is equal to the specified object. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Returns a hash code for the instance of the [`ExtendedAttributeDefinition`](../extendedattributedefinition) class. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Removes a value from the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](./valuelist). |

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
