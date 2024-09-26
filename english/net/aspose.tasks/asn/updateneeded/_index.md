---
title: Asn.UpdateNeeded
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Determines whether the resource assigned to a task needs to be updated as to the status of the task
type: docs
weight: 580
url: /net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Determines whether the resource assigned to a task needs to be updated as to the status of the task.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Examples

Shows how to read/write Asn.UpdateNeeded property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


