---
title: Class ExtendedAttribute
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ExtendedAttribute class. Represents extended attributes
type: docs
weight: 520
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
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Gets the attribute definition. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Gets or sets a value for attributes with date types (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Gets or sets value for attributes with 'Duration' type. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Gets the id of a field. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Gets or sets a value indicating whether a flag is set for an attribute with 'Flag' type. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Gets whether calculation of extended attribute's value resulted in an error. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Gets or sets a value for attributes with numeric types (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Gets or sets a value for attributes with 'Text' type. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Gets the guid of a lookup value. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Gets a value indicating whether a value of this `ExtendedAttribute` instance is read-only. returns true if a formula or rollup is defined in the [`ExtendedAttributeDefinition`](../extendedattributedefinition/) for this object. |

## Methods

| Name | Description |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Returns short string representation of an extended attribute. |

## Remarks

Currently supported all types of Extended attributes reading from MSP Xml 2003/2007 and mpp 2003. For MSP mpp 2007 all Extended attributes reading supported except durations and flags.

## Examples

Shows how to add custom field which value is calculated using formula specified by the user.

```csharp
var project = new Project();

// create new task extended attribute definition
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Add a formula to the attribute.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Create extended attribute
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// We set the Formula for the extended attribute, so it is read only (the value is calculated using formula).
// Output is "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// You can try to set value of read only field, but it will not have effect.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


