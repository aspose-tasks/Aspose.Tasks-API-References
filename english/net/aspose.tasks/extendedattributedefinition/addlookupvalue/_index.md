---
title: ExtendedAttributeDefinition.AddLookupValue
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Adds a value to the internal lookup list. This is a preferable way for manipulations with the ValueList
type: docs
weight: 300
url: /net/aspose.tasks/extendedattributedefinition/addlookupvalue/
---
## ExtendedAttributeDefinition.AddLookupValue method

Adds a value to the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](../valuelist/).

```csharp
public void AddLookupValue(Value value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | Value | Value to add into lookup. |

## Remarks

This method works only for [`ExtendedAttributeDefinition`](../) instances which have [`CalculationType`](../calculationtype/) equals to Lookup.

## Examples

Use this code to add new Value to lookup list:

```csharp
taskTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
```

Shows how to add extended attributes with lookups for assignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Assign resource "1 TRG: Trade Group" to the "TASK 1" by creating a ResourceAssignment object.
var resource = project.Resources.GetById(1);
var task = project.RootTask.Children.GetById(1);
var assignment = project.ResourceAssignments.Add(task, resource);

// Create custom attribute definition with lookup.
var resExtendedAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(
    CustomFieldType.Cost,
    ExtendedAttributeResource.Cost5,
    "My lookup resource cost");
project.ExtendedAttributes.Add(resExtendedAttributeDefinition);

var firstValue = new Value { NumericValue = 1500, Description = "Val 1", Id = 1, Val = "1500" };
var secondValue = new Value { NumericValue = 2500, Description = "Val 2", Id = 2 };
resExtendedAttributeDefinition.AddLookupValue(firstValue);
resExtendedAttributeDefinition.AddLookupValue(secondValue);

// This value can be seen in "Resource usage" view of MS Project.
var attributeValue = resExtendedAttributeDefinition.CreateExtendedAttribute(firstValue);
assignment.ExtendedAttributes.Add(attributeValue);

// Create custom attribute definition with lookup.
var taskCostAttr = ExtendedAttributeDefinition.CreateLookupTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost4, "My lookup task cost");
project.ExtendedAttributes.Add(taskCostAttr);
var taskFirstValue = new Value { NumericValue = 18, Description = "Task val 1", Id = 3, Val = "18" };
var resSecondValue = new Value { NumericValue = 30, Description = "Task val 2", Id = 4 };
var taskWrongValue = new Value { NumericValue = 99, Description = "Task val Wrong", Id = 5, Val = "18" };

taskCostAttr.AddLookupValue(taskFirstValue);
resExtendedAttributeDefinition.AddLookupValue(resSecondValue);

// This value can be seen in "Task usage" view of MS Project.
assignment.ExtendedAttributes.Add(taskCostAttr.CreateExtendedAttribute(taskFirstValue));

// a wrong values can be removed later
taskCostAttr.RemoveLookupValue(taskWrongValue);

// working with project...
```

### See Also

* class [Value](../../value/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


