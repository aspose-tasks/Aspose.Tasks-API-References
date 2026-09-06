---
title: "Resource.Get"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Resource. Retourne la valeur à laquelle la propriété est mappée dans ce conteneur"
type: docs
weight: 830
url: /fr/net/aspose.tasks/resource/get/
---
## Resource.Get&lt;T&gt; method

Renvoie la valeur à laquelle la propriété est mappée dans ce conteneur.

```csharp
public T Get<T>(Key<T, RscKey> key)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Rsc`](../../rsc/) pour obtenir la clé de propriété. |

### Valeur de retour

la valeur à laquelle la propriété est mappée dans ce conteneur.

## Exemples

Montre comment lire/écrire les propriétés de ressource communes.

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
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


