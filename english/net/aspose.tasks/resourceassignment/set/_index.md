---
title: ResourceAssignment.Set
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignment method. Maps the specified property to the specified value in this container
type: docs
weight: 750
url: /net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

Maps the specified property to the specified value in this container.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| Parameter | Description |
| --- | --- |
| T | the type of the mapped value. |
| key | the specified property key. [`Asn`](../../asn/) for getting the property key. |
| val | the value. |

## Examples

Shows how to create an assignment and get/set common assignment properties.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


