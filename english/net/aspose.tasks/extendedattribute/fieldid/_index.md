---
title: ExtendedAttribute.FieldId
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttribute property. Gets the id of a field
type: docs
weight: 40
url: /net/aspose.tasks/extendedattribute/fieldid/
---
## ExtendedAttribute.FieldId property

Gets the id of a field.

```csharp
public string FieldId { get; }
```

## Examples

Shows how to change attribute definition of the extended attribute.

```csharp
var project = new Project();

// create new task extended attribute definition
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// add a formula to the attribute.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// create extended attribute
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// create a new date extended attribute definition
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// add a formula to the attribute.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### See Also

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


