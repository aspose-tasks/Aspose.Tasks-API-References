---
title: "Asn.Milestone"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si l'affectation est un jalon"
type: docs
weight: 330
url: /fr/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

Détermine si l'affectation est un jalon.

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## Exemples

Montre comment lire la propriété Asn.Milestone.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


