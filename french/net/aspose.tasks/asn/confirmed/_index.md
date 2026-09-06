---
title: "Asn.Confirmed"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si une ressource a accepté toutes ses affectations"
type: docs
weight: 170
url: /fr/net/aspose.tasks/asn/confirmed/
---
## Asn.Confirmed field

Détermine si une ressource a accepté toutes ses affectations.

```csharp
public static readonly Key<bool, AsnKey> Confirmed;
```

## Exemples

Montre comment lire/écrire la propriété Asn.Confirmed.

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

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


