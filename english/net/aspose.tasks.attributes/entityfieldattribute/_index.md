---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Attributes.EntityFieldAttribute class. Represents an attribute for entity properties
type: docs
weight: 70
url: /net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Represents an attribute for entity properties.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Constructors

| Name | Description |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | The default constructor. |

## Remarks

Attribute used for [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) and [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) entity properties only, and simplifies it's enumeration.

## Examples

How to enumerate properties using **EntityField** attribute:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### See Also

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


