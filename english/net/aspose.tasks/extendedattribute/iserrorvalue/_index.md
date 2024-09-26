---
title: ExtendedAttribute.IsErrorValue
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttribute property. Gets whether calculation of extended attributes value resulted in an error
type: docs
weight: 60
url: /net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Gets whether calculation of extended attribute's value resulted in an error.

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


