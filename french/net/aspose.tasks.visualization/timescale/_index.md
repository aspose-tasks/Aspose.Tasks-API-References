---
title: "Enum Timescale"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Visualization.Timescale enum. Définit les options qui spécifient comment rendre l'échelle de temps dans les vues Utilisation des tâches du diagramme de Gantt ou Utilisation des ressources lorsque le projet est exporté vers un format graphique."
type: docs
weight: 3430
url: /fr/net/aspose.tasks.visualization/timescale/
---
## Timescale enumeration

Définit les options qui spécifient comment rendre l'échelle de temps dans les vues Diagramme de Gantt, Utilisation des tâches ou Utilisation des ressources lorsque le projet est exporté vers un format graphique.

```csharp
public enum Timescale
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DefinedInView | `0` | Utilisez les paramètres d'échelle de temps définis dans les propriétés de la vue du projet : [`BottomTimescaleTier`](../../aspose.tasks/ganttchartview/bottomtimescaletier/), [`MiddleTimescaleTier`](../../aspose.tasks/ganttchartview/middletimescaletier/), [`TopTimescaleTier`](../../aspose.tasks/ganttchartview/toptimescaletier/). Valide pour les formats qui contiennent des données de vue. Par exemple, les projets qui sont lus au format MPP. |
| Days | `1` | Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un jour. |
| ThirdsOfMonths | `10` | Échelle de temps à deux niveaux prédéfinie où le niveau de détail est d'un tiers de mois. |
| Months | `30` | Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un mois. |

## Exemples

Montre comment enregistrer le projet en tant que fichier SVG.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
SaveOptions options = new SvgOptions
                        {
                            // définissez le <see cref="P:Aspose.Tasks.Saving.SaveOptions.PresentationFormat" /> dans lequel le document sera enregistré
                            PresentationFormat = PresentationFormat.GanttChart,

                            // définissez une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu
                            FitContent = true,

                            // définissez la période de temps minimale à rendre. La valeur par défaut est <see cref="P:Aspose.Tasks.Saving.SaveOptions.Timescale">Jours</see>
                            Timescale = Timescale.ThirdsOfMonths,

                            // détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet
                            // Actuellement, l'utilisation d'un pinceau dégradé n'est pas prise en charge pour le rendu en SVG.
                            // UseGradientBrush = true
                        };
project.Save(OutDir + "UseSvgOptions_out.svg", options);
```

### Voir aussi

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


