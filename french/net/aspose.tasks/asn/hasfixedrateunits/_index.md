---
title: "Asn.HasFixedRateUnits"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si les unités ont un taux fixe"
type: docs
weight: 270
url: /fr/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

Détermine si les unités ont un taux fixe.

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## Exemples

Montre comment lire/écrire la propriété Asn.HasFixedRateUnits.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


