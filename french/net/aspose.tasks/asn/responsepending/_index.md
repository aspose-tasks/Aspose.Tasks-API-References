---
title: "Asn.ResponsePending"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si la réponse a été reçue pour un message TeamAssign"
type: docs
weight: 480
url: /fr/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

Détermine si la réponse a été reçue pour un message TeamAssign.

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## Exemples

Montre comment lire/écrire la propriété Asn.ResponsePending.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


