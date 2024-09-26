---
title: Asn.RegularWork
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The amount of a nonovertime work scheduled for an assignment
type: docs
weight: 420
url: /net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

The amount of a non-overtime work scheduled for an assignment.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Examples

Shows how to read/write Asn.RegularWork property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


