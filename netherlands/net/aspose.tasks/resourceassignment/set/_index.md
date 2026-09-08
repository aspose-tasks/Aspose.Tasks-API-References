---
title: "ResourceAssignment.Set"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "ResourceAssignment methode. Koppelt de opgegeven eigenschap aan de opgegeven waarde in deze container"
type: docs
weight: 750
url: /nl/net/aspose.tasks/resourceassignment/set/
---
## ResourceAssignment.Set&lt;T&gt; method

Kent de opgegeven eigenschap toe aan de opgegeven waarde in deze container.

```csharp
public void Set<T>(Key<T, AsnKey> key, T val)
```

| Parameter | Beschrijving |
| --- | --- |
| T | het type van de gekoppelde waarde. |
| key | de opgegeven eigenschapssleutel. [`Asn`](../../asn/) voor het verkrijgen van de eigenschapssleutel. |
| waarde | de waarde. |

## Voorbeelden

Toont hoe een toewijzing te maken en algemene toewijzings‑eigenschappen op te halen/instellen.

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

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


