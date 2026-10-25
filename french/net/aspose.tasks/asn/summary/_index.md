---
title: "Asn.Summary"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si la tâche est une tâche de résumé"
type: docs
weight: 530
url: /fr/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

Détermine si la tâche est une tâche de synthèse.

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## Exemples

Montre comment lire la propriété Asn.Summary.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


