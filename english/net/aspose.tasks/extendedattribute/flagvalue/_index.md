---
title: ExtendedAttribute.FlagValue
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttribute property. Gets or sets a value indicating whether a flag is set for an attribute with Flag type
type: docs
weight: 50
url: /net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

Gets or sets a value indicating whether a flag is set for an attribute with 'Flag' type.

```csharp
public bool FlagValue { get; set; }
```

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Thrown if the [`AttributeDefinition`](../attributedefinition/) property is not initialized or current attribute is not a flag attribute. |

## Examples

Shows how to create boolean extended attribute.

```csharp
var project = new Project();

// create new task extended attribute definition
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// add a formula to the attribute.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// create extended attribute
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### See Also

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


