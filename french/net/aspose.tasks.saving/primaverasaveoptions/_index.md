---
title: "Classe PrimaveraSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.PrimaveraSaveOptions class. Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera XER."
type: docs
weight: 2150
url: /fr/net/aspose.tasks.saving/primaverasaveoptions/
---
## PrimaveraSaveOptions class

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera XER.

```csharp
public class PrimaveraSaveOptions : SimpleSaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PrimaveraSaveOptions](primaverasaveoptions/)() | Initialise une nouvelle instance de la classe `PrimaveraSaveOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ActivityIdIncrement](../../aspose.tasks.saving/primaverasaveoptions/activityidincrement/) { get; set; } | Obtient ou définit l'incrément utilisé lors du renumérotage des ID d'activité. |
| [ActivityIdPrefix](../../aspose.tasks.saving/primaverasaveoptions/activityidprefix/) { get; set; } | Obtient ou définit le préfixe utilisé lors du renumérotage des ID d'activité. |
| [ActivityIdSuffix](../../aspose.tasks.saving/primaverasaveoptions/activityidsuffix/) { get; set; } | Obtient ou définit le suffixe utilisé lors du renumérotage des ID d'activité. |
| [RenumberActivityIds](../../aspose.tasks.saving/primaverasaveoptions/renumberactivityids/) { get; set; } | Obtient ou définit une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [SkipSummaryAssignments](../../aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/) { get; set; } | Obtient ou définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |

## Exemples

Montre comment travailler avec &lt;see cref=\"Aspose.Tasks.Saving.PrimaveraSaveOptions\" /&gt;.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

// créez les options d'enregistrement Primavera et ajustez-les
var options = new PrimaveraSaveOptions
                  {
                      // définissez le préfixe et le suffixe d'une activité
                      ActivityIdPrefix = "TEST",
                      ActivityIdSuffix = 10000,

                      // contrôlez le renumérotage des activités
                      ActivityIdIncrement = 5,
                      RenumberActivityIds = true
                  };

project.Save(OutDir + "WorkWithPrimaveraSaveOptions_out.xer", options);
```

### Voir aussi

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


