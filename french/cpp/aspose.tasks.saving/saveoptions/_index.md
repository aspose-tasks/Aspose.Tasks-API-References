---
title: "classe Aspose::Tasks::Saving::SaveOptions"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks pour C++"
description: "Il s'agit d'une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier des options supplémentaires lors de l'enregistrement d'un projet dans un format particulier."
type: docs
weight: 10
url: /fr/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Il s'agit d'une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier des options supplémentaires lors de l'enregistrement d'un projet dans un format particulier.

Une instance de toute classe dérivée de la classe SaveOptions est transmise aux surcharges Save de flux ou Save de chaîne afin que l'utilisateur définisse des options personnalisées lors de l'enregistrement d'un document.

## Méthodes

| Nom | Description |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Obtient la liste des instances de la classe BarStyle qui apparaissent dans la vue du projet. |
| [get_CustomPageSize](./get_custompagesize/) | Obtient la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Obtient une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est VRAI). |
| [get_EndDate](./get_enddate/) | Obtient une date jusqu'à laquelle terminer le rendu. |
| [get_FitContent](./get_fitcontent/) | Obtient une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Obtient si une section calendrier d'une vue doit être rendue jusqu'à la fin (côté droit) de la dernière page. Si la valeur est false, la section calendrier est rendue exactement jusqu'à EndDate, même s'il y a un espace vide sur une page. |
| [get_Gridlines](./get_gridlines/) | Obtient une liste de Gridline qui apparaissent dans la vue du projet. |
| [get_IsPortrait](./get_isportrait/) | Obtient une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Obtient une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Obtient un tableau de PageLegendItem qui définissent quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Obtient une valeur indiquant si les tâches critiques doivent être affichées en couleur rouge (la valeur par défaut est FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Obtient la couleur du temps non travaillé. |
| [get_PageCount](./get_pagecount/) | Obtient le nombre de pages du projet. |
| [get_PageSize](./get_pagesize/) | Obtient la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Obtient le PresentationFormat dans lequel le document sera enregistré. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Obtient une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu tienne sur une page. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Obtient une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations sur les barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées. |
| [get_StartDate](./get_startdate/) | Obtient la date à partir de laquelle commencer le rendu. |
| [get_TextStyles](./get_textstyles/) | Obtient la liste des styles de texte appliqués lors du rendu d'une vue de projet. |
| [get_Timescale](./get_timescale/) | Obtient la valeur Timescale qui est utilisée pour contrôler comment l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Obtient un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Obtient une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| [get_View](./get_view/) | Obtient une liste des colonnes de vue à rendre ( GanttChartColumn ). Si non définies, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et ViewSettings sont définies, les colonnes de View remplacent celles de ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Obtient une vue ( View ) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété Visualization::PresentationFormat est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants (( Aspose::Tasks::View::Screen )) : (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | Définit la liste des instances de la classe BarStyle qui apparaissent dans la vue du projet. |
| [set_CustomPageSize](./set_custompagesize/) | Définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |
| [set_EndDate](./set_enddate/) | Définit une date jusqu'à laquelle le rendu doit se terminer. |
| [set_FitContent](./set_fitcontent/) | Définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Définit si une section calendrier d'une vue doit être rendue jusqu'à la fin (côté droit) de la dernière page. Si la valeur est false, la section calendrier est rendue exactement jusqu'à EndDate, même s'il reste un espace vide sur la page. |
| [set_Gridlines](./set_gridlines/) | Définit une liste de Gridline qui apparaissent dans la vue du projet. |
| [set_IsPortrait](./set_isportrait/) | Définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Définit une valeur qui détermine comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Définit un tableau de PageLegendItem qui spécifie quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Définit la couleur du temps non travaillé. |
| [set_PageSize](./set_pagesize/) | Définit la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Définit le PresentationFormat dans lequel le document sera enregistré. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu tienne sur une page. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Yes pour que les sous‑tâches puissent être agrégées. |
| [set_StartDate](./set_startdate/) | Définit la date à partir de laquelle le rendu doit commencer. |
| [set_TextStyles](./set_textstyles/) | Définit la liste des styles de texte appliqués lors du rendu d'une vue de projet. |
| [set_Timescale](./set_timescale/) | Définit la valeur Timescale qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Définit un comportement qui détermine comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| [set_View](./set_view/) | Définit une liste des colonnes de vue à rendre ( GanttChartColumn ). Si non définies, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et ViewSettings sont définies, les colonnes de View remplacent celles de ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Définit une vue ( View ) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété Visualization::PresentationFormat est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants (( Aspose::Tasks::View::Screen )) : (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

