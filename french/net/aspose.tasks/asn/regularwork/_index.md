---
title: "Asn.RegularWork"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Le montant d'un travail non supplémentaire prévu pour une affectation"
type: docs
weight: 420
url: /fr/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

La quantité de travail hors heures supplémentaires prévue pour une affectation.

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## Exemples

Montre comment lire/écrire la propriété Asn.RegularWork.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


