---
title: "Asn.Milestone"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn-veld. Bepaalt of de toewijzing een mijlpaal is"
type: docs
weight: 330
url: /nl/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Bepaalt of de opdracht een mijlpaal is.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Voorbeelden

Toont hoe de eigenschap Asn.Milestone te lezen.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


