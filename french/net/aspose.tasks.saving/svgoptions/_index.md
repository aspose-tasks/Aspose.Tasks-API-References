---
title: "Classe SvgOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.Saving.SvgOptions class. Permet de spécifier des options supplémentaires lors du rendu des pages du projet en SVG"
type: docs
weight: 2230
url: /fr/net/aspose.tasks.saving/svgoptions/
---
## SvgOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages de projet au format SVG.

```csharp
public class SvgOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [SvgOptions](svgoptions/)() | Initialise une nouvelle instance de la classe `SvgOptions` qui peut être utilisée pour enregistrer le projet au format SVG. |

## Propriétés

| Nom | Description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtient ou définit la liste des instances de la classe [`BarStyle`](../../aspose.tasks.visualization/barstyle/) qui apparaissent dans la vue du projet. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtient ou définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtient ou définit une date jusqu'à laquelle terminer le rendu. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtient ou définit une liste de [`Gridline`](../../aspose.tasks.visualization/gridline/) qui apparaissent dans la vue du projet. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Obtient ou définit une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Obtient ou définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtient ou définit la couleur du temps non travaillé. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtient ou définit le nombre de pages du projet. |
| [PageSavingCallback](../../aspose.tasks.saving/svgoptions/pagesavingcallback/) { get; set; } | Obtient ou définit un rappel d'implémentation défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtient ou définit la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtient ou définit le [`PresentationFormat`](../saveoptions/presentationformat/) dans lequel le document sera enregistré. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtient ou définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu tienne sur une page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtient ou définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtient ou définit la date à partir de laquelle le rendu commence. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Obtient ou définit un rappel qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtient ou définit la liste des styles de texte appliqués lors du rendu d'une vue de projet. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtient ou définit la valeur [`Timescale`](../saveoptions/timescale/) qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Obtient ou définit un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| override [UseGradientBrush](../../aspose.tasks.saving/svgoptions/usegradientbrush/) { get; set; } | Détermine s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. Actuellement, l'utilisation d'un pinceau dégradé n'est pas prise en charge pour le rendu en SVG. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtient ou définit une liste des colonnes de vue à rendre ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Si non défini, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et [`ViewSettings`](../saveoptions/viewsettings/) sont toutes deux définies, les colonnes de View remplacent celles de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtient ou définit une vue ([`View`](../saveoptions/view/)) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

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

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


