---
title: "Classe PrimaveraXmlSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Saving.PrimaveraXmlSaveOptions. Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format XML Primavera"
type: docs
weight: 2160
url: /fr/net/aspose.tasks.saving/primaveraxmlsaveoptions/
---
## PrimaveraXmlSaveOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format XML Primavera.

```csharp
public class PrimaveraXmlSaveOptions : SimpleSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraXmlSaveOptions](primaveraxmlsaveoptions/)() | Initialise une nouvelle instance de la classe `PrimaveraXmlSaveOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [SaveRootTask](../../aspose.tasks.saving/primaveraxmlsaveoptions/saveroottask/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut enregistrer une tâche racine ou non. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/) { get; set; } | Obtient ou définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |

## Exemples

Montre comment exporter le fichier XML Primavera.

```csharp
var project = new Project(DataDir + "project.xml");

var options = new PrimaveraXmlSaveOptions();
options.SaveRootTask = false;
project.Save(OutDir + "UsingPrimaveraXMLSaveOptions_out.xml", options);
```

### Voir aussi

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


