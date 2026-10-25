---
title: "SaveOptions"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 130
url: /fr/python-net/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

Il s'agit d'une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier des options supplémentaires lors de l'enregistrement d'un projet<br/>            dans un format particulier.

Le type SaveOptions expose les membres suivants :
## Propriétés
| Nom | Description |
| :- | :- |
| save_format | Obtient ou définit le format dans lequel le document sera enregistré si cet objet d'options d'enregistrement est utilisé. |
| bar_styles | Obtient ou définit la liste des instances de la classe [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/) qui apparaissent dans la vue du projet. |
| draw_non_working_time | Obtient ou définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |
| end_date | Obtient ou définit une date jusqu'à laquelle terminer le rendu. |
| timescale_fit_behavior | Obtient ou définit un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| fit_content | Obtient ou définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| gridlines | Obtient ou définit une liste de [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/) qui apparaissent dans la vue du projet. |
| legend_drawing_options | Obtient ou définit une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage. |
| legend_items | Obtient ou définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de page.<br/>            Si null, les éléments par défaut sont rendus. |
| mark_critical_tasks | Obtient ou définit une valeur indiquant si les tâches critiques doivent être affichées en couleur rouge (Valeur par défaut : FALSE). |
| non_working_time_color | Obtient ou définit la couleur du temps non travaillé. |
| page_count | Obtient ou définit le nombre de pages du projet. |
| page_size | Obtient ou définit la taille de la page à rendre (Valeur par défaut : PageSize.A4). |
| is_portrait | Obtient ou définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| presentation_format | Obtient ou définit le [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/) dans lequel le document sera enregistré. |
| roll_up_gantt_bars | Obtient ou définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées.<br/>            Pour les sous‑tâches, le champ Rollup indique si les informations sur les barres Gantt des sous‑tâches seront agrégées dans la barre de tâche récapitulative.<br/>            Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées.<br/>            Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées. |
| start_date | Obtient ou définit la date à partir de laquelle commencer le rendu. |
| text_styles | Obtient ou définit la liste des styles de texte appliqués lors du rendu d’une vue de projet. |
| timescale | Obtient ou définit la valeur du [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) utilisée pour contrôler la façon dont l’échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| use_gradient_brush | Obtient ou définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| view | Obtient ou définit une liste des colonnes de vue à rendre ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Si non définies, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus.<br/>            Si les propriétés View et [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) sont toutes deux définies, les colonnes de View remplacent celles de ViewSettings. |
| view_settings | Obtient ou définit une vue ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image.<br/>            Si cette propriété est définie, la propriété [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) est ignorée lors de l’enregistrement du projet.<br/>            La vue doit provenir de l’un des écrans suivants (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| render_to_single_page | Obtient ou définit une valeur indiquant si un projet doit être rendu sur une seule page<br/>            lorsque le projet est enregistré au format graphique.<br/>            La taille de la page sera modifiée afin que le projet rendu puisse tenir sur une page. |

### Voir aussi

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

