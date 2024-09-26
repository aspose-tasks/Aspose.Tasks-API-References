---
title: Prj.UpdateManuallyScheduledTasksWhenEditingLinks
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. Determines whether manual tasks must be updated when links were edited
type: docs
weight: 770
url: /net/aspose.tasks/prj/updatemanuallyscheduledtaskswheneditinglinks/
---
## Prj.UpdateManuallyScheduledTasksWhenEditingLinks field

Determines whether manual tasks must be updated when links were edited.

```csharp
public static readonly Key<NullableBool, PrjKey> UpdateManuallyScheduledTasksWhenEditingLinks;
```

## Examples

Shows how to read/write Prj.UpdateManuallyScheduledTasksWhenEditingLinks property.

```csharp
var project = new Project();

project.Set(Prj.UpdateManuallyScheduledTasksWhenEditingLinks, true);

Console.WriteLine("Update Manually Scheduled Tasks When Editing Links: " + project.Get(Prj.UpdateManuallyScheduledTasksWhenEditingLinks));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


