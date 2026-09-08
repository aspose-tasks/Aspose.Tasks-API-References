---
title: "Asn.Confirmed"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Asn veld. Bepaalt of een resource al zijn toewijzingen heeft geaccepteerd"
type: docs
weight: 170
url: /nl/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Bepaalt of een resource al zijn opdrachten heeft geaccepteerd.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Voorbeelden

Toont hoe de eigenschap Asn.Confirmed te lezen/schrijven.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


