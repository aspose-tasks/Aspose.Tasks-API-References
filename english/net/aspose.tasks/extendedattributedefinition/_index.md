---
title: ExtendedAttributeDefinition
second_title: Aspose.Tasks for .NET API Reference
description: 
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
| [Alias](alias) { get; set; } | Gets or sets the alias of a custom field. |
| [AppendNewValues](appendnewvalues) { get; set; } | Gets or sets a value indicating whether new values added to a project are automatically added to the list. |
| [AutoRollDown](autorolldown) { get; set; } | Gets or sets a value indicating whether an automatic roll down to assignments is enabled. |
| [CalculationType](calculationtype) { get; set; } | Gets or sets the type of calculation of the custom attribute's value. |
| [CfType](cftype) { get; } | Gets the type of a custom field. |
| [Default](default) { get; set; } | Gets or sets the default value in the list. |
| [DefaultGuid](defaultguid) { get; set; } | Gets or sets the Guid of the default lookup table entry. |
| [ElementType](elementtype) { get; set; } | Gets or sets the extended attribute is associated with a task, a resource or an assignment. |
| [FieldId](fieldid) { get; set; } | Gets or sets corresponds to the project id of a custom field. Use string representation of a constant from [`ExtendedAttributeTask`](../extendedattributetask) class to specify [`FieldId`](./fieldid) property. |
| [FieldName](fieldname) { get; } | Gets the name of a custom field. |
| [Formula](formula) { get; set; } | Gets or sets the formula that Microsoft Project uses to populate a custom task field. |
| [Guid](guid) { get; set; } | Gets or sets the Guid of a custom field. |
| [LookupUid](lookupuid) { get; } | Gets a Guid of the lookup table associated with a custom field. |
| [MaxMultiValues](maxmultivalues) { get; set; } | Gets or sets the maximum number of values you can set in a pick list. |
| [ParentProject](parentproject) { get; } | Gets the parent project for the [`ExtendedAttributeDefinition`](../extendedattributedefinition) instance. |
| [PhoneticsAlias](phoneticsalias) { get; set; } | Gets or sets the phonetic pronunciation of the alias of a custom field. |
| [RestrictValues](restrictvalues) { get; set; } | Gets or sets a value indicating whether the custom field values are restricted to values in the [`ValueList`](./valuelist). |
| [RollupType](rolluptype) { get; set; } | Gets or sets the way rollups are calculated. |
| [SecondaryGuid](secondaryguid) { get; set; } | Gets or sets the secondary guid of extended attribute. |
| [SecondaryPid](secondarypid) { get; set; } | Gets or sets the secondary PID of a custom field. |
| [SummaryRowsCalculationType](summaryrowscalculationtype) { get; set; } | Gets or sets the type of calculation of the custom attribute's value for summary rows. |
| [UserDef](userdef) { get; set; } | Gets or sets a value indicating whether a custom field is user defined. |
| [ValueList](valuelist) { get; } | Gets the List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](valuelistsortorder) { get; set; } | Gets or sets the way value lists are sorted. Values are: 0=Descending, 1=Ascending. |

## Methods

| Name | Description |
| --- | --- |
| static [CreateLookupResourceDefinition](createlookupresourcedefinition)(ExtendedAttributeResource, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Resources only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateLookupResourceDefinition](createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Resources only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateLookupTaskDefinition](createlookuptaskdefinition)(ExtendedAttributeTask, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Tasks only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateLookupTaskDefinition](createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](./calculationtype) equals to Lookup and can be used in Tasks only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateResourceDefinition](createresourcedefinition)(ExtendedAttributeResource, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Resource only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id. |
| static [CreateResourceDefinition](createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Resource only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method. |
| static [CreateTaskDefinition](createtaskdefinition)(ExtendedAttributeTask, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Tasks only. You are required to specify *fieldId* and *alias* when calling this method. The field type is inferred from field id. |
| static [CreateTaskDefinition](createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](./calculationtype) equals to None and can be used in Tasks only. You are required to specify *customFieldType*, *fieldId* and *alias* when calling this method. |
| [AddLookupValue](addlookupvalue)(Value) | Adds a value to the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](./valuelist). |
| [CreateExtendedAttribute](createextendedattribute)() | Creates a new extended attribute with the field ID which equals to this object's field ID value. |
| [CreateExtendedAttribute](createextendedattribute)(bool) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified flag value. |
| [CreateExtendedAttribute](createextendedattribute)(DateTime) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified date value. |
| [CreateExtendedAttribute](createextendedattribute)(decimal) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified numeric value. |
| [CreateExtendedAttribute](createextendedattribute)(Duration) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified duration value. |
| [CreateExtendedAttribute](createextendedattribute)(string) | Creates a new extended attribute with the field ID which equals to this object's field ID value and the specified text value. |
| [CreateExtendedAttribute](createextendedattribute)(Value) | Creates new extended attribute linked with specified [`Value`](../value) item. |
| override [Equals](equals)(object) | Returns a flag indicating whether this instance is equal to the specified object. |
| override [GetHashCode](gethashcode)() | Returns a hash code for the instance of the [`ExtendedAttributeDefinition`](../extendedattributedefinition) class. |
| [RemoveLookupValue](removelookupvalue)(Value) | Removes a value from the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](./valuelist). |

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
