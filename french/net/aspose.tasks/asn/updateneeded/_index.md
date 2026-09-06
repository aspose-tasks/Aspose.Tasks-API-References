---
title: "Asn.UpdateNeeded"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si la ressource affectée à une tâche doit être mise à jour concernant le statut de la tâche"
type: docs
weight: 580
url: /fr/net/aspose.tasks/asn/updateneeded/
---
## Asn.UpdateNeeded field

Détermine si la ressource affectée à une tâche doit être mise à jour concernant le statut de la tâche.

```csharp
public static readonly Key<bool, AsnKey> UpdateNeeded;
```

## Exemples

Montre comment lire/écrire la propriété Asn.UpdateNeeded.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.UpdateNeeded, true);

Console.WriteLine("Update Needed: " + assignment.Get(Asn.UpdateNeeded));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


