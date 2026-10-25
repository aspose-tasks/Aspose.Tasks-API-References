---
title: "SaveTemplateOptions.RemoveResourceRates"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété SaveTemplateOptions. Obtient ou définit une valeur indiquant si les taux de ressources d'un modèle de projet doivent être supprimés"
type: docs
weight: 50
url: /fr/net/aspose.tasks.saving/savetemplateoptions/removeresourcerates/
---
## SaveTemplateOptions.RemoveResourceRates property

Obtient ou définit une valeur indiquant si les taux de ressources d'un modèle de projet doivent être supprimés.

```csharp
public bool RemoveResourceRates { get; set; }
```

## Exemples

Montre comment enregistrer un projet en tant que modèle en utilisant des options.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var projectFileInfo = Project.GetProjectFileInfo(DataDir + "EstimatedMilestoneTasks.mpp");

Console.WriteLine("Project File Format: " + projectFileInfo.ProjectFileFormat);

// créer des options d'enregistrement de modèle
// et ajuster ses propriétés
var options = new SaveTemplateOptions
{
    // définir une valeur indiquant si tous les coûts fixes d'un modèle de projet doivent être supprimés
    RemoveFixedCosts = true,

    // définir une valeur indiquant si toutes les valeurs réelles d'un modèle de projet doivent être supprimées
    RemoveActualValues = true,

    // définir une valeur indiquant si les taux de ressources d'un modèle de projet doivent être supprimés
    RemoveResourceRates = true,

    // définir une valeur indiquant si toutes les valeurs de référence d'un modèle de projet doivent être supprimées
    RemoveBaselineValues = true
};

project.SaveAsTemplate(OutDir + "SaveProjectDataAsTemplate_out.mpt", options);

var templateFileInfo = Project.GetProjectFileInfo(DataDir + "SaveProjectDataAsTemplate_out.mpt");
Console.WriteLine("Project File Format: " + templateFileInfo.ProjectFileFormat);
```

### Voir aussi

* class [SaveTemplateOptions](../)
* namespace [Aspose.Tasks.Saving](../../savetemplateoptions/)
* assembly [Aspose.Tasks](../../../)


