---
title: "Asn.Uid"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. L'identifiant unique d'une affectation"
type: docs
weight: 560
url: /fr/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

L'identifiant unique d'une affectation.

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## Exemples

Montre comment lire/écrire la propriété Asn.Uid.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


