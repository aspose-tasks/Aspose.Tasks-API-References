---
title: Asn.VAC
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The difference between baseline cost and total cost
type: docs
weight: 590
url: /net/aspose.tasks/asn/vac/
---
## Asn.VAC field

The difference between baseline cost and total cost.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Examples

Shows how to read Asn.VAC property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


