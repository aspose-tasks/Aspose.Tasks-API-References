---
title: Class ExtendedAttributeCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ExtendedAttributeCollection class. Represents a collection of ExtendedAttribute objects
type: docs
weight: 530
url: /net/aspose.tasks/extendedattributecollection/
---
## ExtendedAttributeCollection class

Represents a collection of [`ExtendedAttribute`](../extendedattribute/) objects.

```csharp
public class ExtendedAttributeCollection : IList<ExtendedAttribute>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributecollection/count/) { get; } | Gets the number of elements contained in this collection. |
| [IsReadOnly](../../aspose.tasks/extendedattributecollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read-only; otherwise, false. |
| [Item](../../aspose.tasks/extendedattributecollection/item/) { get; set; } | Gets or sets the element at the specified index. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributecollection/add/)(ExtendedAttribute) | Adds the specified item to this collection. |
| [Clear](../../aspose.tasks/extendedattributecollection/clear/)() | Removes all items from this collection. |
| [Contains](../../aspose.tasks/extendedattributecollection/contains/)(ExtendedAttribute) | Returns true if the specified item is found in this collection; otherwise, false. |
| [CopyTo](../../aspose.tasks/extendedattributecollection/copyto/)(ExtendedAttribute[], int) | Copies the elements of this collection to the specified array, starting at the specified array index. |
| [GetEnumerator](../../aspose.tasks/extendedattributecollection/getenumerator/)() | Returns an enumerator for this collection. |
| [IndexOf](../../aspose.tasks/extendedattributecollection/indexof/)(ExtendedAttribute) | Determines the index of the specified item in this collection. |
| [Insert](../../aspose.tasks/extendedattributecollection/insert/)(int, ExtendedAttribute) | Inserts the specified item at the specified index. |
| [Remove](../../aspose.tasks/extendedattributecollection/remove/)(ExtendedAttribute) | Removes the first occurrence of a specific object from this collection. |
| [RemoveAt](../../aspose.tasks/extendedattributecollection/removeat/)(int) | Removes an item at the specified index. |

## Examples

Shows how to use extended attribute collections.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Get zero index task
var task = project.RootTask.Children.GetById(1);

if (!task.ExtendedAttributes.IsReadOnly && task.ExtendedAttributes.Count > 0)
{
    // clear extended attributes
    task.ExtendedAttributes.Clear();
}

// create extended attribute definition for a task
var taskDefinition1 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
var taskDefinition2 = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Finish, ExtendedAttributeTask.Finish7, "Finish 7");
project.ExtendedAttributes.Add(taskDefinition1);
project.ExtendedAttributes.Add(taskDefinition2);

Console.WriteLine("Iterate over task extended attributes of " + task.Get(Tsk.Name) + " task: ");
foreach (var attribute in task.ExtendedAttributes)
{
    Console.WriteLine("Attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

// Add extended attribute 1
var extendedAttribute1 = taskDefinition1.CreateExtendedAttribute();
extendedAttribute1.DateValue = new DateTime(2020, 4, 14, 8, 0, 0);
if (task.ExtendedAttributes.IndexOf(extendedAttribute1) < 0)
{
    task.ExtendedAttributes.Insert(0, extendedAttribute1);
}

// Add extended attribute 2
var extendedAttribute2 = taskDefinition2.CreateExtendedAttribute();
extendedAttribute2.DateValue = new DateTime(2020, 4, 14, 17, 0, 0);
task.ExtendedAttributes.Add(extendedAttribute2);

// work with extended attributes...

// remove extended attribute by index
task.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Count of task's extended attributes: " + task.ExtendedAttributes.Count);

// use collection index access
Console.WriteLine("Attribute 1 Value: " + task.ExtendedAttributes[0].DateValue);

var otherProject = new Project();
var otherTask = otherProject.RootTask.Children.Add("Other task");

// copy attributes to other project
var attributes = new ExtendedAttribute[task.ExtendedAttributes.Count];
task.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherTask.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other task's extended attributes: ");
foreach (var attribute in otherTask.ExtendedAttributes)
{
    Console.WriteLine("Other attribute FieldId: " + attribute.FieldId);
    Console.WriteLine("Other attribute Value: " + attribute.DateValue);
    Console.WriteLine();
}

if (task.ExtendedAttributes.Contains(extendedAttribute2))
{
    task.ExtendedAttributes.Remove(extendedAttribute2);
}

// remove all extended attribute definitions
while (otherTask.ExtendedAttributes.Count > 0)
{
    otherTask.ExtendedAttributes.Remove(otherTask.ExtendedAttributes[0]);
}
```

### See Also

* class [ExtendedAttribute](../extendedattribute/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


