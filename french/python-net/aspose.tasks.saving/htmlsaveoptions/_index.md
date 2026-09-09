---
title: "HtmlSaveOptions"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 20
url: /fr/python-net/aspose.tasks.saving/htmlsaveoptions/
---

## HtmlSaveOptions class

Permet de spécifier des options supplémentaires lors du rendu des pages du projet au format HTML.

Le type HtmlSaveOptions expose les membres suivants :
## Constructeurs
| Nom | Description |
| :- | :- |
| HtmlSaveOptions() | Initialise une nouvelle instance de la classe [HtmlSaveOptions](/tasks/python-net/aspose.tasks.saving/htmlsaveoptions/). |
## Propriétés
| Nom | Description |
| :- | :- |
| save_format |  |
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
| use_gradient_brush | Obtient ou définit une valeur indiquant s’il faut utiliser un pinceau dégradé lors du rendu de la mise en page du projet. |
| view | Obtient ou définit une liste des colonnes de vue à rendre ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Si non définies, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus.<br/>            Si les propriétés View et [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) sont toutes deux définies, les colonnes de View remplacent celles de ViewSettings. |
| view_settings | Obtient ou définit une vue ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image.<br/>            Si cette propriété est définie, la propriété [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) est ignorée lors de l’enregistrement du projet.<br/>            La vue doit provenir de l’un des écrans suivants (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Obtient ou définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| render_to_single_page | Obtient ou définit une valeur indiquant si un projet doit être rendu sur une seule page<br/>            lorsque le projet est enregistré au format graphique.<br/>            La taille de la page sera modifiée afin que le projet rendu puisse tenir sur une page. |
| css_style_prefix | Obtient ou définit le préfixe de style CSS. |
| font_settings | Spécifie les paramètres de police utilisés lors du rendu de la vue du projet. |
| reduce_footer_gap | Obtient ou définit une valeur indiquant si l'écart entre la dernière tâche et le pied de page doit être réduit. |
| include_project_name_in_page_header | Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans l'en-tête de page HTML. |
| include_project_name_in_title | Obtient ou définit une valeur indiquant s'il faut inclure le nom du projet dans le titre HTML. |
| pages | Obtient ou définit une liste de numéros de page à enregistrer lors du rendu de la mise en page du projet. |
| export_css | Obtient ou définit la manière dont le CSS est exporté. |
| export_images | Obtient ou définit la manière dont les images sont exportées. |
| export_fonts | Obtient ou définit la manière dont les polices sont exportées. |
| css_saving_callback | Obtient ou définit le rappel qui est appelé pour créer la ressource de stockage du CSS. |
| font_saving_callback | Obtient ou définit le rappel qui est appelé pour créer la ressource de stockage de la police. |
| image_saving_callback | Obtient ou définit le rappel qui est appelé pour créer la ressource de stockage de la police. |
| font_face_types | Obtient ou définit les types de police. |
| page_saving_callback | Obtient ou définit un rappel défini par l'utilisateur qui est utilisé pour obtenir un flux de sortie pour chaque page rendue. |

### Voir aussi

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

