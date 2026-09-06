---
title: "Asn.Resource"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. La ressource affectée à une tâche"
type: docs
weight: 470
url: /fr/net/aspose.tasks/asn/resource/
---
## Asn.Resource field

La ressource affectée à une tâche.

```csharp
public static readonly Key<Resource, AsnKey> Resource;
```

## Exemples

Montre comment lire les propriétés Asn.Task et Asn.Resource.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Resource](../../resource/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


