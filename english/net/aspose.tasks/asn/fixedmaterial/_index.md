---
title: Asn.FixedMaterial
second_title: Aspose.Tasks for .NET API Reference
description: Asn field. Determines whether the consumption of an assigned material resource occurs in a single fixed amount
type: docs
weight: 260
url: /net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Determines whether the consumption of an assigned material resource occurs in a single, fixed amount.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Examples

Shows how to read/write Asn.FixedMaterial property.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


