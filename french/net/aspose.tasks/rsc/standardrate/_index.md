---
title: "Rsc.StandardRate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le taux de rémunération pour le travail régulier non supplémentaire effectué par une ressource"
type: docs
weight: 620
url: /fr/net/aspose.tasks/rsc/standardrate/
---
## Rsc.StandardRate field

Le taux de rémunération pour le travail régulier, non supplémentaire, effectué par une ressource.

```csharp
public static readonly Key<decimal, RscKey> StandardRate;
```

## Exemples

Montre comment gérer les taux et les groupes de ressources.

```csharp
var project = new Project(DataDir + "UpdateResourceData.mpp");

// Ajouter une ressource et définir certaines propriétés
var resource = project.Resources.Add("Rsc");
resource.Set(Rsc.Start, new DateTime(2020, 4, 1, 8, 0, 0));
resource.Set(Rsc.StandardRate, 30);
resource.Set(Rsc.OvertimeRate, 45);
resource.Set(Rsc.Group, "Workgroup1");

Console.WriteLine("Resource Start: " + resource.Get(Rsc.Start));
Console.WriteLine("Resource Standard Rate: " + resource.Get(Rsc.StandardRate));
Console.WriteLine("Resource Overtime Rate: " + resource.Get(Rsc.OvertimeRate));
Console.WriteLine("Resource Group: " + resource.Get(Rsc.Group));

project.Save(OutDir + "UpdateResourceData_out.mpp", SaveFileFormat.Mpp);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


