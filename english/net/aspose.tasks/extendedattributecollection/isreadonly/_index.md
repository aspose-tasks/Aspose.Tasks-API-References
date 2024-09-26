---
title: ExtendedAttributeCollection.IsReadOnly
second_title: Aspose.Tasks for .NET API Reference
description: ExtendedAttributeCollection property. Gets a value indicating whether this collection is readonly otherwise false
type: docs
weight: 20
url: /net/aspose.tasks/extendedattributecollection/isreadonly/
---
## ExtendedAttributeCollection.IsReadOnly property

Gets a value indicating whether this collection is read-only; otherwise, false.

```csharp
public bool IsReadOnly { get; }
```

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

* class [ExtendedAttributeCollection](../)
* namespace [Aspose.Tasks](../../extendedattributecollection/)
* assembly [Aspose.Tasks](../../../)


