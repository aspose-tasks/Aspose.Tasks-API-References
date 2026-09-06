---
title: "Classe MPPSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Saving.MPPSaveOptions. Permet de spécifier des options supplémentaires lors de la sauvegarde des données du projet au format MPP"
type: docs
weight: 2050
url: /fr/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement des données du projet au format MPP.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | Initialise une nouvelle instance de la classe `MPPSaveOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut supprimer les données de macros VBA existantes lors de l'enregistrement d'un projet au format MPP. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | Obtient ou définit un mot de passe utilisé pour protéger le fichier MPP résultant. Actuellement, il est pris en charge pour les formats MS Project 2010 et ultérieurs. Une valeur null indique que le fichier de projet n'est pas protégé. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut supprimer les affectations de ressources invalides lors de l'enregistrement au format MPP. MS Project crée une affectation de ressource vide pour chaque tâche. Définissez ce drapeau sur true pour les supprimer lors de l'enregistrement. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. Les données de filtre comprennent les collections Project.TaskFilters et Project.ResourceFilters. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut écrire les données de groupes lors de l'enregistrement d'un projet au format MPP. Les données de groupe comprennent les collections Project.TaskGroups et Project.ResourceGroups. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut mettre à jour les données de macros VBA existantes dans le fichier MPP. L'écriture de VbaModule.SourceCode est actuellement prise en charge. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut écrire les données de vue lors de l'enregistrement d'un projet au format MPP. Les données de vue comprennent les collections Project.Views, Filters et Tables. |

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

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


