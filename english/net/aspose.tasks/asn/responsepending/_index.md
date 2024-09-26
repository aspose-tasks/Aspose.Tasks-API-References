---
title: Asn.ResponsePending
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Determines whether the response has been received for a TeamAssign message
type: docs
weight: 480
url: /net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

Determines whether the response has been received for a TeamAssign message.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Examples

Shows how to read/write Asn.ResponsePending property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


