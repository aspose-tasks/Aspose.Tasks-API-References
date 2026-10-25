---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceAssignment. Définit les unités pour l'affectation d'une ressource matérielle avec une consommation de matériel variable. La consommation de matériel variable signifie que, à mesure que la durée de l'affectation change, la quantité de matériaux utilisée change proportionnellement."
type: docs
weight: 760
url: /fr/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

Définit les unités pour l'affectation d'une ressource matérielle avec une consommation de matériel variable. La consommation de matériel variable signifie que, à mesure que la durée de l'affectation change, la quantité de matériaux utilisée change proportionnellement.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| unités | Double | Nombre d'unités accumulées pendant la période. |
| rateScaleType | RateScaleType | Période pendant laquelle la valeur de l'unité est accumulée. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Si la méthode est appelée pour l'affectation d'une ressource non matérielle. |

## Remarques

Par exemple, pour définir '123/mois', SetUnitsScaled(123D, RateScaleType.Month) doit être appelé.

## Exemples

Montre comment définir une consommation de matériel variable (par ex. '10/jour' ou '1/semaine') pour une affectation d'une ressource matérielle.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supposons que nous voulions définir une consommation de matériel '1/semaine'.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### Voir aussi

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


