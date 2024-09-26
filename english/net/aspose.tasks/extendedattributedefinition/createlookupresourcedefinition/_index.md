---
title: ExtendedAttributeDefinition.CreateLookupResourceDefinition
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Factory method which creates an extended attribute definition with lookup. It has CalculationType equals to Lookup and can be used in Resources only. You are required to specify fieldId and alias when call this method. The field type is inferred from field id
type: docs
weight: 10
url: /net/aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/
---
## CreateLookupResourceDefinition(ExtendedAttributeResource, string) {#createlookupresourcedefinition_1}

Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](../calculationtype/) equals to Lookup and can be used in Resources only. You are required to specify *fieldId* and *alias* when call this method. The field type is inferred from field id.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldId | ExtendedAttributeResource | The specified [`ExtendedAttributeResource`](../../extendedattributeresource/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *fieldId* and *alias*.

## Examples

Use this example to create a custom field definition for a resource with lookup and then fill it with text values:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
```

Shows how to write updated extended attribute definitions.

```csharp
var project = new Project(DataDir + "WriteUpdatedExtendedAttributeDefinitions.mpp");

// Add new text3 extended attribute with lookup and one lookup value
var definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Text3, "New text3 attribute");
definition.ElementType = ElementType.Task;
project.ExtendedAttributes.Add(definition);

var textVal = new Value
{
    Id = 1,
    Description = "Text value descr",
    Val = "Text value1"
};

definition.AddLookupValue(textVal);

// Add new cost1 extended attribute with lookup and two cost values
var taskCostAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Cost1, "New cost1 attribute");
project.ExtendedAttributes.Add(taskCostAttributeDefinition);

var costVal1 = new Value
{
    Id = 2,
    Description = "Cost value 1 descr",
    Val = "99900"
};

var costVal2 = new Value
{
    Id = 3,
    Description = "Cost value 2 descr",
    Val = "11100"
};

taskCostAttributeDefinition.AddLookupValue(costVal1);
taskCostAttributeDefinition.AddLookupValue(costVal2);

// Add new task and assign attribute lookup value.
var task = project.RootTask.Children.Add("New task");

var taskAttr = taskCostAttributeDefinition.CreateExtendedAttribute(costVal1);
task.ExtendedAttributes.Add(taskAttr);

var taskStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Start7, "New start 7 attribute");

var startVal = new Value
{
    Id = 4,
    DateTimeValue = DateTime.Now,
    Description = "Start 7 value description"
};

taskStartAttributeDefinition.AddLookupValue(startVal);

project.ExtendedAttributes.Add(taskStartAttributeDefinition);

var taskFinishAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Finish4, "New finish 4 attribute");

var finishVal = new Value
{
    Id = 5,
    DateTimeValue = DateTime.Now,
    Description = "Finish 4 value description"
};

taskFinishAttributeDefinition.ValueList.Add(finishVal);

project.ExtendedAttributes.Add(taskFinishAttributeDefinition);

var numberAttributeDefinition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(ExtendedAttributeTask.Number20, "New number attribute");

var val1 = new Value
{
    Id = 6,
    Val = "1",
    Description = "Number 1 value"
};
var val2 = new Value
{
    Id = 7,
    Val = "2",
    Description = "Number 2 value"
};
var val3 = new Value();
val2.Id = 8;
val3.Val = "3";
val3.Description = "Number 3 value";

numberAttributeDefinition.AddLookupValue(val1);
numberAttributeDefinition.AddLookupValue(val2);
numberAttributeDefinition.AddLookupValue(val3);

project.ExtendedAttributes.Add(numberAttributeDefinition);

var rscStartAttributeDefinition = ExtendedAttributeDefinition.CreateLookupResourceDefinition(ExtendedAttributeResource.Start5, "New start5 attribute");

var value = new Value
{
    Id = 9,
    DateTimeValue = DateTime.Now,
    Description = "this is start5 value descr"
};

rscStartAttributeDefinition.AddLookupValue(value);

project.ExtendedAttributes.Add(rscStartAttributeDefinition);

// Define a duration attribute without lookup.
var taskDurationAttributeDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration1, "New Duration");
project.ExtendedAttributes.Add(taskDurationAttributeDefinition);

// Add new task and assign duration value to the previously defined duration attribute.
var timeTask = project.RootTask.Children.Add("New task");

var durationExtendedAttribute = taskDurationAttributeDefinition.CreateExtendedAttribute();

durationExtendedAttribute.DurationValue = project.GetDuration(3.0, TimeUnitType.Hour);
timeTask.ExtendedAttributes.Add(durationExtendedAttribute);

var options = new MPPSaveOptions
{
    WriteViewData = true
};

project.Save(OutDir + "WriteUpdatedExtendedAttributeDefinitions_out.mpp", options);
```

### See Also

* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateLookupResourceDefinition(CustomFieldType, ExtendedAttributeResource, string) {#createlookupresourcedefinition}

Factory method which creates an extended attribute definition with lookup. It has [`CalculationType`](../calculationtype/) equals to Lookup and can be used in Resources only. You are required to specify *customFieldType*, *fieldId* and *alias* when call this method.

```csharp
public static ExtendedAttributeDefinition CreateLookupResourceDefinition(
    CustomFieldType customFieldType, ExtendedAttributeResource fieldId, string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | CustomFieldType | The specified [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeResource | The specified [`ExtendedAttributeResource`](../../extendedattributeresource/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *customFieldType*, *fieldId* and *alias*.

## Examples

Use this example to create a custom field definition for a resource with lookup and then fill it with text values:

```csharp
var resourceTextAttr = ExtendedAttributeDefinition.CreateLookupResourceDefinition(CustomFieldType.Text, ExtendedAttributeResource.Text27, "My custom field");
resourceTextAttr.AddLookupValue(new Value { Id = 1, Val = "Text value 1", Description = "Text value description 1" });
resourceTextAttr.AddLookupValue(new Value { Id = 2, Val = "Text value 2", Description = "Text value description 2" });
project.ExtendedAttributes.Add(resourceTextAttr);
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

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeResource](../../extendedattributeresource/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


