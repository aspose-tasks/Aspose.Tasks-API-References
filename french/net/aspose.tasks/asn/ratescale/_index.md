---
title: "Asn.RateScale"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Asn. L'unité de temps pour le taux d'utilisation de l'affectation de ressource matérielle. Retourne 0 si non définie"
type: docs
weight: 410
url: /fr/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

L'unité de temps pour le taux d'utilisation de l'affectation de ressource matérielle. Retourne 0 si non définie.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## Exemples

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


