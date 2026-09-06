---
title: "Asn.VAC"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La différence entre le coût de référence et le coût total"
type: docs
weight: 590
url: /fr/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

La différence entre le coût de référence et le coût total.

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## Exemples

Montre comment lire la propriété Asn.VAC.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


