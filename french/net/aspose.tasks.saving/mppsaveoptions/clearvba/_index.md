---
title: "MPPSaveOptions.ClearVba"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut supprimer les données des macros VBA existantes lors de l'enregistrement d'un projet au format MPP."
type: docs
weight: 20
url: /fr/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

Obtient ou définit une valeur indiquant s'il faut supprimer les données de macros VBA existantes lors de l'enregistrement d'un projet au format MPP.

```csharp
public bool ClearVba { get; set; }
```

## Exemples

Montre comment supprimer les macros VBA d'un fichier MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### Voir aussi

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


