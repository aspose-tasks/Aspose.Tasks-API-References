---
title: "Class SaveTemplateOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.SaveTemplateOptions class. Permet de spécifier des options supplémentaires lors de l'enregistrement d'un projet en tant que modèle"
type: docs
weight: 2200
url: /fr/net/aspose.tasks.saving/savetemplateoptions/
---
## SaveTemplateOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement d'un projet en tant que modèle.

```csharp
public class SaveTemplateOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SaveTemplateOptions](savetemplateoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [RemoveActualValues](../../aspose.tasks.saving/savetemplateoptions/removeactualvalues/) { get; set; } | Obtient ou définit une valeur indiquant si toutes les valeurs réelles d'un modèle de projet doivent être supprimées. |
| [RemoveBaselineValues](../../aspose.tasks.saving/savetemplateoptions/removebaselinevalues/) { get; set; } | Obtient ou définit une valeur indiquant si toutes les valeurs de référence d'un modèle de projet doivent être supprimées. |
| [RemoveFixedCosts](../../aspose.tasks.saving/savetemplateoptions/removefixedcosts/) { get; set; } | Obtient ou définit une valeur indiquant si tous les coûts fixes d'un modèle de projet doivent être supprimés. |
| [RemoveResourceRates](../../aspose.tasks.saving/savetemplateoptions/removeresourcerates/) { get; set; } | Obtient ou définit une valeur indiquant si les taux de ressources d'un modèle de projet doivent être supprimés. |

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

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


