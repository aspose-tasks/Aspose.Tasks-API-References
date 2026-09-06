---
title: "MPPSaveOptions.WriteViewData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. Les données de vue incluent les collections Project.Views Filters et Tables."
type: docs
weight: 80
url: /fr/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

Obtient ou définit une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. Les données de vue comprennent les collections Project.Views, Filters et Tables.

```csharp
public bool WriteViewData { get; set; }
```

## Exemples

Montre comment enregistrer le projet dans un flux en tant que fichier MPP.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // créer des options d'enregistrement
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP
        RemoveInvalidAssignments = true
    };

    // enregistrer le MPP avec des options
    project.Save(stream, options);
}
```

### Voir aussi

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


