---
title: "Resource.Set"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Resource. Associe la propriété spécifiée à la valeur spécifiée dans ce conteneur"
type: docs
weight: 860
url: /fr/net/aspose.tasks/resource/set/
---
## Set&lt;T&gt;(Key&lt;T, RscKey&gt;, T) {#set_1}

Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

```csharp
public void Set<T>(Key<T, RscKey> key, T val)
```

| Paramètre | Description |
| --- | --- |
| T | le type de la valeur mappée. |
| key | la clé de propriété spécifiée. [`Rsc`](../../rsc/) pour obtenir la clé de propriété. |
| val | la valeur. |

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

---

## Set(Key&lt;DateTime, RscKey&gt;, DateTime) {#set}

Mappe la propriété spécifiée à la valeur spécifiée dans ce conteneur.

```csharp
public void Set(Key<DateTime, RscKey> key, DateTime val)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| key | Key`2 | la clé de propriété spécifiée. [`Rsc`](../../rsc/) pour obtenir la clé de propriété. |
| val | DateTime | la valeur. |

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


