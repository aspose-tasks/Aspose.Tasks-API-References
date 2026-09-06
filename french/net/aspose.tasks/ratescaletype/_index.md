---
title: "Énumération RateScaleType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Énumération Aspose.Tasks.RateScaleType. Spécifie le type d'échelle de taux"
type: docs
weight: 1650
url: /fr/net/aspose.tasks/ratescaletype/
---
## RateScaleType enumeration

Spécifie le type d'échelle de taux.

```csharp
public enum RateScaleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `0` | Indique le type d'échelle de taux Non défini. |
| Minute | `1` | Indique le type d'échelle de taux Minute. |
| Hour | `2` | Indique le type d'échelle de taux Heure. |
| Day | `3` | Indique le type d'échelle de taux Jour. |
| Week | `4` | Indique le type d'échelle de taux Semaine. |
| Month | `5` | Indique le type d'échelle de taux Mois. |
| Quarter | `6` | Indique le type d'échelle de taux Trimestre. |
| Year | `7` | Indique le type d'échelle de taux Année. |

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

Montre comment travailler avec l'échelle de taux d'une affectation lorsque nous voulons définir une consommation de matériel variable (par ex. '10/jour' ou '1/semaine') pour une affectation d'une ressource matérielle.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// Supposons que nous voulions définir une consommation de matériel '1/semaine'.
// Nous devrions définir le taux horaire sur la propriété Units, donc nous divisons 1D par les heures par semaine.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// Veuillez noter qu'à partir de la version 24.4, cela peut être fait en appelant une méthode :
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// Seules les affectations de ressources matérielles peuvent avoir une valeur d'échelle de taux non nulle.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


