---
title: Asn.CostRateTableType
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. The cost rate table used for this assignment
type: docs
weight: 190
url: /net/aspose.tasks/asn/costratetabletype/
---
## Asn.CostRateTableType field

The cost rate table used for this assignment.

```csharp
public static readonly Key<RateType, AsnKey> CostRateTableType;
```

## Examples

Shows how to read/write Asn.CostRateTableType property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.CostRateTableType, RateType.B);

Console.WriteLine("Cost Rate Table Type: " + assignment.Get(Asn.CostRateTableType));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateType](../../ratetype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


