---
title: "Classe PdfSaveOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Saving.PdfSaveOptions. Permet de spécifier des options supplémentaires lors du rendu des pages de projet au format PDF"
type: docs
weight: 2130
url: /fr/net/aspose.tasks.saving/pdfsaveoptions/
---
## PdfSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages du projet en PDF.

```csharp
public class PdfSaveOptions : SaveOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [PdfSaveOptions](pdfsaveoptions/)() | Initialise une nouvelle instance de la classe `PdfSaveOptions` qui peut être utilisée pour enregistrer un document au format [`PDF`](../savefileformat/). |

## Propriétés

| Nom | Description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtient ou définit la liste des instances de la classe [`BarStyle`](../../aspose.tasks.visualization/barstyle/) qui apparaissent dans la vue du projet. |
| [Compliance](../../aspose.tasks.saving/pdfsaveoptions/compliance/) { get; set; } | Obtient ou définit le niveau de conformité souhaité pour le document PDF généré. La valeur par défaut est Pdf15. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [DigitalSignatureDetails](../../aspose.tasks.saving/pdfsaveoptions/digitalsignaturedetails/) { get; set; } | Obtient ou définit les détails de la signature numérique. Si non défini, aucune signature ne sera effectuée. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtient ou définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |
| [EncryptionDetails](../../aspose.tasks.saving/pdfsaveoptions/encryptiondetails/) { get; set; } | Obtient ou définit les détails du chiffrement. Si non défini, aucun chiffrement ne sera effectué. |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtient ou définit une date jusqu'à laquelle terminer le rendu. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [FontSettings](../../aspose.tasks.saving/pdfsaveoptions/fontsettings/) { get; } | Spécifie les paramètres de police utilisés lors du rendu de la vue du projet. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtient ou définit une liste de [`Gridline`](../../aspose.tasks.visualization/gridline/) qui apparaissent dans la vue du projet. |
| [IsPortrait](../../aspose.tasks.saving/saveoptions/isportrait/) { get; set; } | Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [LegendDrawingOptions](../../aspose.tasks.saving/saveoptions/legenddrawingoptions/) { get; set; } | Obtient ou définit une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage. |
| [LegendItems](../../aspose.tasks.saving/saveoptions/legenditems/) { get; set; } | Obtient ou définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus. |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtient ou définit la couleur du temps non travaillé. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtient ou définit le nombre de pages du projet. |
| [Pages](../../aspose.tasks.saving/pdfsaveoptions/pages/) { get; set; } | Obtient ou définit la liste des numéros de pages à enregistrer lors de la sauvegarde de la mise en page du projet dans des fichiers séparés. Toutes les pages seront enregistrées si cette liste est vide. |
| [PageSavingCallback](../../aspose.tasks.saving/pdfsaveoptions/pagesavingcallback/) { get; set; } | Obtient ou définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. Applicable lorsque l'option [`SaveToSeparateFiles`](./savetoseparatefiles/) est utilisée. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtient ou définit la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtient ou définit le [`PresentationFormat`](../saveoptions/presentationformat/) dans lequel le document sera enregistré. |
| [ReduceFooterGap](../../aspose.tasks.saving/pdfsaveoptions/reducefootergap/) { get; set; } | Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtient ou définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu tienne sur une page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtient ou définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [SaveToSeparateFiles](../../aspose.tasks.saving/pdfsaveoptions/savetoseparatefiles/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut enregistrer les pages du projet dans des fichiers séparés. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtient ou définit la date à partir de laquelle le rendu commence. |
| [TaskLinkDrawingCallback](../../aspose.tasks.saving/saveoptions/tasklinkdrawingcallback/) { get; set; } | Obtient ou définit un rappel qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le diagramme de feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes Gantt, feuille de tâches et utilisation des tâches. |
| [TextCompression](../../aspose.tasks.saving/pdfsaveoptions/textcompression/) { get; set; } | Obtient ou définit le type de compression à utiliser pour tous les flux de contenu sauf les images. La valeur par défaut est Flate. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtient ou définit la liste des styles de texte appliqués lors du rendu d'une vue de projet. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtient ou définit la valeur [`Timescale`](../saveoptions/timescale/) qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [TimescaleFitBehavior](../../aspose.tasks.saving/saveoptions/timescalefitbehavior/) { get; set; } | Obtient ou définit un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush/) { get; set; } | Obtient ou définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtient ou définit une liste des colonnes de vue à rendre ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/)). Si non défini, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et [`ViewSettings`](../saveoptions/viewsettings/) sont toutes deux définies, les colonnes de View remplacent celles de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtient ou définit une vue ([`View`](../saveoptions/view/)) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété [`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants (([`Screen`](../../aspose.tasks/view/screen/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |

## Exemples

Montre comment enregistrer les pages sélectionnées d'un projet dans un fichier PDF.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");
var options = new PdfSaveOptions();
options.RenderToSinglePage = false;
options.Pages = new List<int>();

// vérifions le nombre de pages pouvant être exportées
Console.WriteLine("Page Count: " + options.PageCount);

options.Pages.Add(1);
options.Pages.Add(4);
project.Save(OutDir + "SaveToMultiplePDFFiles_out.pdf", options);
```

### Voir aussi

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


