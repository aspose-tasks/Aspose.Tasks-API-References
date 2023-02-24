---
title: Class HtmlSaveOptions
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.Saving.HtmlSaveOptions classe. Permet de spécifier des options supplémentaires lors du rendu des pages de projet au format HTML.
type: docs
weight: 1750
url: /fr/net/aspose.tasks.saving/htmlsaveoptions/
---
## HtmlSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages de projet au format HTML.

```csharp
public class HtmlSaveOptions : SaveOptions
```

## Constructeurs

| Nom | La description |
| --- | --- |
| [HtmlSaveOptions](htmlsaveoptions/)() | Initialise une nouvelle instance du`HtmlSaveOptions` classe. |

## Propriétés

| Nom | La description |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles/) { get; set; } | Obtient ou définit la liste des instances du[`BarStyle`](../../aspose.tasks.visualization/barstyle/) classe qui apparaissent dans la vue du projet. |
| [CssSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/csssavingcallback/) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker CSS. |
| [CssStylePrefix](../../aspose.tasks.saving/htmlsaveoptions/cssstyleprefix/) { get; set; } | Obtient ou définit le préfixe de style CSS. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize/) { get; set; } | Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [DefaultFontName](../../aspose.tasks.saving/htmlsaveoptions/defaultfontname/) { get; set; } | Obtient ou définit la police par défaut pour le rendu. |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime/) { get; set; } | Obtient ou définit une valeur indiquant si les périodes chômées doivent être dessinées (la valeur par défaut est TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate/) { get; set; } | Obtient ou définit une date à laquelle terminer le rendu. |
| [ExportCss](../../aspose.tasks.saving/htmlsaveoptions/exportcss/) { get; set; } | Obtient ou définit la manière dont les CSS sont exportés. |
| [ExportFonts](../../aspose.tasks.saving/htmlsaveoptions/exportfonts/) { get; set; } | Obtient ou définit la manière dont les polices sont exportées. |
| [ExportImages](../../aspose.tasks.saving/htmlsaveoptions/exportimages/) { get; set; } | Obtient ou définit la façon dont les images sont exportées. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent/) { get; set; } | Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.saving/saveoptions/fittimescaletoendofpage/) { get; set; } | Obtient ou définit si une section de calendrier d'une vue doit être rendue à la fin (côté droit) de la dernière page. Si la valeur est false, la section de calendrier est rendue exactement à EndDate, même s'il y a un espace vide sur une page. |
| [FontFaceTypes](../../aspose.tasks.saving/htmlsaveoptions/fontfacetypes/) { get; set; } | Obtient ou définit les types de polices. |
| [FontResolveCallback](../../aspose.tasks.saving/htmlsaveoptions/fontresolvecallback/) { get; set; } | Obtient ou définit un rappel qui peut être utilisé pour personnaliser les polices résolues. |
| [FontSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/fontsavingcallback/) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker la police. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines/) { get; set; } | Obtient ou définit une liste de[`Gridline`](../../aspose.tasks.visualization/gridline/) qui apparaissent dans la vue du projet. |
| [ImageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/imagesavingcallback/) { get; set; } | Obtient ou définit le rappel appelé pour créer une ressource pour stocker la police. |
| [IncludeProjectNameInPageHeader](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameinpageheader/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de la page HTML. |
| [IncludeProjectNameInTitle](../../aspose.tasks.saving/htmlsaveoptions/includeprojectnameintitle/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage/) { get; set; } | Obtient ou définit une valeur indiquant si la légende doit être affichée sur chaque page (la valeur par défaut est TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks/) { get; set; } | Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor/) { get; set; } | Obtient ou définit la couleur des périodes chômées. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount/) { get; } | Obtient ou définit le nombre de pages du projet. |
| [Pages](../../aspose.tasks.saving/htmlsaveoptions/pages/) { get; set; } | Obtient ou définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. Toutes les pages du projet seront enregistrées si cette liste est vide. |
| [PageSavingCallback](../../aspose.tasks.saving/htmlsaveoptions/pagesavingcallback/) { get; set; } | Obtient ou définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize/) { get; set; } | Obtient ou définit la taille de la page à afficher (la valeur par défaut est PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat/) { get; set; } | Obtient ou définit le[`PresentationFormat`](../saveoptions/presentationformat/) dans lequel le document sera enregistré. |
| [ReduceFooterGap](../../aspose.tasks.saving/htmlsaveoptions/reducefootergap/) { get; set; } | Obtient ou définit une valeur indiquant si un écart entre la dernière tâche et le pied de page doit être réduit. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage/) { get; set; } | Obtient ou définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu puisse tenir sur une seule page. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars/) { get; set; } | Obtient ou définit une valeur indiquant si les sous-tâches de la barre des tâches récapitulatives doivent être marquées. Pour les sous-tâches, le champ Cumul indique si les informations sur les barres du Gantt des sous-tâches seront reportées dans la barre des tâches récapitulatives. Pour les tâches récapitulatives, le champ Cumul Le champ indique si la barre des tâches récapitulatives affiche des barres cumulées. Le champ Cumul des tâches récapitulatives doit être défini sur Oui pour que les sous-tâches puissent y être cumulées. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat/) { get; } | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate/) { get; set; } | Obtient ou définit la date à partir de laquelle le rendu commence. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer/) { get; set; } | Obtient ou définit le comparateur pour trier les tâches sur le diagramme de Gantt et le tableau de la feuille de tâches. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter/) { get; set; } | Obtient ou définit la condition utilisée pour filtrer les tâches rendues sur les diagrammes de Gantt, de feuille de tâches et d'utilisation des tâches. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles/) { get; set; } | Obtient ou définit la liste des instances du[`TextStyle`](../../aspose.tasks.visualization/textstyle/) classe qui apparaissent dans la vue du projet. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale/) { get; set; } | Obtient ou définit le[`Timescale`](../saveoptions/timescale/) valeur qui est utilisée pour contrôler la façon dont l'échelle de temps (le cas échéant) est rendue lorsque le projet est enregistré au format graphique. |
| override [UseGradientBrush](../../aspose.tasks.saving/htmlsaveoptions/usegradientbrush/) { get; set; } | Obtient ou définit une valeur indiquant s'il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. L'utilisation actuelle du pinceau dégradé n'est pas prise en charge lors du rendu au format HTML. |
| [UseProjectDefaultFont](../../aspose.tasks.saving/htmlsaveoptions/useprojectdefaultfont/) { get; set; } | Obtient ou définit une valeur indiquant si la police par défaut doit être utilisée pour le rendu. |
| [View](../../aspose.tasks.saving/saveoptions/view/) { get; set; } | Obtient ou définit une liste des colonnes de vue à afficher ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn/) ). S'ils ne sont pas définis, les identifiants de tâche, les noms de tâche, le début et la fin sont rendus uniquement. Si à la fois Afficher et[`ViewSettings`](../saveoptions/viewsettings/)les propriétés sont définies, les colonnes de View remplacent les colonnes de ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings/) { get; set; } | Obtient ou définit une vue ([`View`](../saveoptions/view/) ) rendre. Vous pouvez utiliser ces options pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat/) La propriété est ignorée lorsque le projet est enregistré. La vue doit provenir de l'un des écrans suivants (([`Screen`](../../aspose.tasks/view/screen/) )) : (Gantt, Feuille de tâches, Utilisation des tâches, Feuille de ressources, Utilisation des ressources) |

### Voir également

* class [SaveOptions](../saveoptions/)
* espace de noms [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* Assemblée [Aspose.Tasks](../../)


