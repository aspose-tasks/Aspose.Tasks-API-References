---
title: Asn.Confirmed
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Determines whether a resource has accepted all of its assignments
type: docs
weight: 170
url: /net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Determines whether a resource has accepted all of its assignments.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Examples

Shows how to read/write Asn.Confirmed property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Confirmed, true);

Console.WriteLine("Confirmed: " + assignment.Get(Asn.Confirmed));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


