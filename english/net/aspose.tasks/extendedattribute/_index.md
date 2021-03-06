---
title: ExtendedAttribute
second_title: Aspose.Tasks for .NET API Reference
description: 
type: docs
weight: 510
url: /net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Represents extended attributes.

```csharp
public class ExtendedAttribute
```

## Properties

| Name | Description |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition) { get; } | Gets the attribute definition. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue) { get; set; } | Gets or sets a value for attributes with date types (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue) { get; set; } | Gets or sets value for attributes with 'Duration' type. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid) { get; } | Gets the id of a field. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue) { get; set; } | Gets or sets a value indicating whether a flag is set for an attribute with 'Flag' type. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue) { get; } | Gets whether calculation of extended attribute's value resulted in an error. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue) { get; set; } | Gets or sets a value for attributes with numeric types (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue) { get; set; } | Gets or sets a value for attributes with 'Text' type. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid) { get; } | Gets the guid of a lookup value. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly) { get; } | Gets a value indicating whether a value of this [`ExtendedAttribute`](../extendedattribute) instance is read-only. returns true if a formula or rollup is defined in the [`ExtendedAttributeDefinition`](../extendedattributedefinition) for this object. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring)() | Returns short string representation of an extended attribute. |

### Remarks

Currently supported all types of Extended attributes reading from MSP Xml 2003/2007 and mpp 2003. For MSP mpp 2007 all Extended attributes reading supported except durations and flags.

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks)
* assembly [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
