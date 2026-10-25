---
title: "SvgOptions.SvgOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur SvgOptions. Initialise une nouvelle instance de la classe SvgOptions qui peut être utilisée pour enregistrer le projet au format SVG"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/svgoptions/svgoptions/
---
## SvgOptions constructor

Initialise une nouvelle instance de la classe [`SvgOptions`](../) qui peut être utilisée pour enregistrer le projet au format SVG.

```csharp
public SvgOptions()
```

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

* class [SvgOptions](../)
* namespace [Aspose.Tasks.Saving](../../svgoptions/)
* assembly [Aspose.Tasks](../../../)


