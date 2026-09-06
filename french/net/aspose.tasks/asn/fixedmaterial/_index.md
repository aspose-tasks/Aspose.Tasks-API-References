---
title: "Asn.FixedMaterial"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. Détermine si la consommation d'une ressource matérielle affectée se produit en un seul montant fixe"
type: docs
weight: 260
url: /fr/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

Détermine si la consommation d'une ressource matérielle assignée se produit en une quantité unique et fixe.

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## Exemples

Montre comment lire/écrire la propriété Asn.FixedMaterial.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


