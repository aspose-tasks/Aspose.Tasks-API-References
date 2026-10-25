---
title: "MPPSaveOptions.RemoveInvalidAssignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. MS Project crée une affectation de ressource vide pour chaque tâche. Définissez ce drapeau sur true pour les supprimer lors de l'enregistrement."
type: docs
weight: 40
url: /fr/net/aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/
---
## MPPSaveOptions.RemoveInvalidAssignments property

Obtient ou définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. MS Project crée une affectation de ressource vide pour chaque tâche. Définissez ce drapeau sur true pour les supprimer lors de l'enregistrement.

```csharp
public bool RemoveInvalidAssignments { get; set; }
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


