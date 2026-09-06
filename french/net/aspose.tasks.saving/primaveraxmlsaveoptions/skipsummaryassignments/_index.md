---
title: "PrimaveraXmlSaveOptions.SkipSummaryAssignments"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété PrimaveraXmlSaveOptions. Obtient ou définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation"
type: docs
weight: 30
url: /fr/net/aspose.tasks.saving/primaveraxmlsaveoptions/skipsummaryassignments/
---
## PrimaveraXmlSaveOptions.SkipSummaryAssignments property

Obtient ou définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Remarques

Le logiciel Primavera ne prend pas en charge les affectations de ressources aux tâches récapitulatives (WBS). Ainsi, l'exportation de telles affectations peut entraîner un fichier invalide selon le modèle de Primavera. Si vrai, les affectations aux tâches récapitulatives sont ignorées lors de l'exportation. Si faux (valeur par défaut), une exception sera levée si une affectation à une tâche récapitulative est rencontrée lors de l'exportation.

## Exemples

Montre comment utiliser le drapeau SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera ne prend pas en charge les affectations de ressources aux tâches récapitulatives.
// Ainsi, l'exportation de telles affectations au format Primavera peut entraîner des fichiers qui ne peuvent pas être importés dans Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Voir aussi

* class [PrimaveraXmlSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaveraxmlsaveoptions/)
* assembly [Aspose.Tasks](../../../)


