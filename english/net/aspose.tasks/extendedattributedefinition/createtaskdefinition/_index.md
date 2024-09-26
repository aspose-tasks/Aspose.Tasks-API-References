---
title: ExtendedAttributeDefinition.CreateTaskDefinition
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeDefinition method. Factory method which creates a simple extended attribute definition which Microsoft Project shows as None. It has CalculationType equals to None and can be used in Tasks only. You are required to specify customFieldType fieldId and alias when calling this method
type: docs
weight: 40
url: /net/aspose.tasks/extendedattributedefinition/createtaskdefinition/
---
## CreateTaskDefinition(CustomFieldType, ExtendedAttributeTask, string) {#createtaskdefinition}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](../calculationtype/) equals to None and can be used in Tasks only. You are required to specify *customFieldType*, *fieldId* and *alias* when calling this method.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(CustomFieldType customFieldType, 
    ExtendedAttributeTask fieldId, string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| customFieldType | CustomFieldType | The specified [`CustomFieldType`](../../customfieldtype/) type. |
| fieldId | ExtendedAttributeTask | The specified [`ExtendedAttributeTask`](../../extendedattributetask/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *customFieldType*, *fieldId* and *alias*.

## Examples

Use this example to create a custom text field definition:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Shows how to create task's extended attributes.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

// Create an Extended Attribute Definition of Text1 type
var taskExtendedAttributeText1Definition =
    ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Task City Name");

// Add it to the project's Extended Attributes collection
project.ExtendedAttributes.Add(taskExtendedAttributeText1Definition);

// Add a task to the project
var task = project.RootTask.Children.Add("Task 1");

// Create an Extended Attribute from the Attribute Definition
var taskExtendedAttributeText1 = taskExtendedAttributeText1Definition.CreateExtendedAttribute();

// Assign a value to the generated Extended Attribute. The type of the attribute is "Text", the "TextValue" property should be used.
taskExtendedAttributeText1.TextValue = "London";

// Add the Extended Attribute to task
task.ExtendedAttributes.Add(taskExtendedAttributeText1);

project.Save(OutDir + "PlainTextExtendedAttribute_out.mpp", SaveFileFormat.Mpp);

var project4 = new Project(DataDir + "Blank2010.mpp");

// Create an Extended Attribute Definition of Text2 type
var taskExtendedAttributeText2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Add lookup values for the extended attribute definition
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1" });
taskExtendedAttributeText2Definition.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2" });

// Add it to the project's Extended Attributes collection
project4.ExtendedAttributes.Add(taskExtendedAttributeText2Definition);

// Add a task to the project
var task2 = project4.RootTask.Children.Add("Task 2");

// Crate an Extended Attribute from the Text2 Lookup Definition for Id 1
var taskExtendedAttributeText2 = taskExtendedAttributeText2Definition.CreateExtendedAttribute(taskExtendedAttributeText2Definition.ValueList[1]);

// Add the Extended Attribute to task
task2.ExtendedAttributes.Add(taskExtendedAttributeText2);

project4.Save(OutDir + "TextExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project2 = new Project(DataDir + "Blank2010.mpp");

// Create an Extended Attribute Definition of Duration2 type
var taskExtendedAttributeDuration2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration2,
    "Some duration");

// Add lookup values for extended attribute definition
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 2, Duration = project2.GetDuration(4, TimeUnitType.Hour), Description = "4 hours" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 3, Duration = project2.GetDuration(1, TimeUnitType.Day), Description = "1 day" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 4, Duration = project2.GetDuration(1, TimeUnitType.Hour), Description = "1 hour" });
taskExtendedAttributeDuration2Definition.AddLookupValue(
    new Value { Id = 7, Duration = project2.GetDuration(10, TimeUnitType.Day), Description = "10 days" });

// Add the definition to the project's Extended Attributes collection
project2.ExtendedAttributes.Add(taskExtendedAttributeDuration2Definition);

// Add a task to the project
var task3 = project2.RootTask.Children.Add("Task 3");

// Create an Extended Attribute from the Duration2 Lookup Definition for Id 3
var taskExtendedAttributeDuration2 =
    taskExtendedAttributeDuration2Definition.CreateExtendedAttribute(taskExtendedAttributeDuration2Definition.ValueList[3]);

// Add the Extended Attribute to task
task3.ExtendedAttributes.Add(taskExtendedAttributeDuration2);

project2.Save(OutDir + "DurationExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);

var project3 = new Project(DataDir + "Blank2010.mpp");

// Create an Extended Attribute Definition of Finish2 Type
var taskExtendedAttributeFinish2Definition = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Finish,
    ExtendedAttributeTask.Finish2,
    "Some finish");

// Add lookup values for extended attribute definition
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 2, DateTimeValue = new DateTime(1984, 01, 01, 00, 00, 01), Description = "This is Value2" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 3, DateTimeValue = new DateTime(1994, 01, 01, 00, 01, 01), Description = "This is Value3" });
taskExtendedAttributeFinish2Definition.AddLookupValue(
    new Value { Id = 4, DateTimeValue = new DateTime(2009, 12, 31, 00, 00, 00), Description = "This is Value4" });
taskExtendedAttributeFinish2Definition.AddLookupValue(new Value { Id = 7, DateTimeValue = DateTime.Now, Description = "This is Value6" });

// Add the definition to the project's Extended Attributes collection
project3.ExtendedAttributes.Add(taskExtendedAttributeFinish2Definition);

// Add a task to the project
var task4 = project3.RootTask.Children.Add("Task 4");

// Create an Extended Attribute from the Finish2 Lookup Definition for Id 3
var taskExtendedAttributeFinish2 = taskExtendedAttributeFinish2Definition.CreateExtendedAttribute(taskExtendedAttributeFinish2Definition.ValueList[3]);

// Add the Extended Attribute to task
task4.ExtendedAttributes.Add(taskExtendedAttributeFinish2);

project3.Save(OutDir + "FinishExtendedAttributeWithLookup_out.mpp", SaveFileFormat.Mpp);
```

### See Also

* enum [CustomFieldType](../../customfieldtype/)
* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)

---

## CreateTaskDefinition(ExtendedAttributeTask, string) {#createtaskdefinition_1}

Factory method which creates a simple extended attribute definition, which Microsoft Project shows as "None". It has [`CalculationType`](../calculationtype/) equals to None and can be used in Tasks only. You are required to specify *fieldId* and *alias* when calling this method. The field type is inferred from field id.

```csharp
public static ExtendedAttributeDefinition CreateTaskDefinition(ExtendedAttributeTask fieldId, 
    string alias)
```

| Parameter | Type | Description |
| --- | --- | --- |
| fieldId | ExtendedAttributeTask | The specified [`ExtendedAttributeTask`](../../extendedattributetask/) field ID. |
| alias | String | The specified String alias. |

### Return Value

Created instance of the [`ExtendedAttributeDefinition`](../) class with specified *fieldId* and *alias*.

## Examples

Use this example to create a custom text field definition:

```csharp
var taskTextAttr = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text27, "My custom field");
project.ExtendedAttributes.Add(taskTextAttr);
```

Shows how to create extended attribute definition and set a string value of the attribute while its constructing.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My Text");
project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 22, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// create extended attribute with a value equals to the 'Common Info'
var extendedAttribute = definition.CreateExtendedAttribute("Common Info");

// add extended attribute initialized by value the 'Common Info'
task.ExtendedAttributes.Add(extendedAttribute);
```

### See Also

* enum [ExtendedAttributeTask](../../extendedattributetask/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


