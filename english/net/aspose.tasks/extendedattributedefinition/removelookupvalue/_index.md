---
title: ExtendedAttributeDefinition.RemoveLookupValue
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Removes a value from the internal lookup list. This is a preferable way for manipulations with the ValueList
type: docs
weight: 340
url: /net/aspose.tasks/extendedattributedefinition/removelookupvalue/
---
## ExtendedAttributeDefinition.RemoveLookupValue method

Removes a value from the internal lookup list. This is a preferable way for manipulations with the [`ValueList`](../valuelist/).

```csharp
public void RemoveLookupValue(Value value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | Value | Value to remove from lookup. |

## Remarks

This method works only for [`ExtendedAttributeDefinition`](../) instances which have [`CalculationType`](../calculationtype/) equals to Lookup.

## Examples

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


