---
title: Asn.Milestone
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Determines whether the assignment is a milestone
type: docs
weight: 330
url: /net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Determines whether the assignment is a milestone.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Examples

Shows how to read Asn.Milestone property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


