---
title: "Rsc.Group"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Rsc. Le groupe auquel une ressource appartient"
type: docs
weight: 300
url: /fr/net/aspose.tasks/rsc/group/
---
## Rsc.Group field

Le groupe auquel une ressource appartient.

```csharp
public static readonly Key<string, RscKey> Group;
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


