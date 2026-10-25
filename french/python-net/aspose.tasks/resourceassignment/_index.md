---
title: "ResourceAssignment"
second_title: "Aspose.Tasks pour Python via .NET Référence de l'API"
description: 
type: docs
weight: 980
url: /fr/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Représente une affectation de ressource dans un projet.

Le type ResourceAssignment expose les membres suivants :
## Propriétés
| Nom | Description |
| :- | :- |
| uid | Obtient ou définit une valeur de Uid. |
| percent_work_complete | Obtient ou définit une valeur de PercentWorkComplete. |
| actual_cost | Obtient ou définit une valeur de ActualCost. |
| actual_finish | Obtient ou définit une valeur de ActualFinish. |
| actual_overtime_cost | Obtient ou définit une valeur de ActualOvertimeCost. |
| actual_start | Obtient ou définit une valeur de ActualStart. |
| actual_work | Obtient ou définit une valeur de ActualWork. |
| acwp | Obtient ou définit une valeur de ACWP. |
| confirmed | Obtient ou définit une valeur indiquant si Confirmed est défini ou non. |
| cost | Obtient ou définit la valeur de Cost. |
| cost_rate_table_type | Obtient ou définit une valeur de CostRateTableType. |
| cost_variance | Obtient ou définit une valeur de CostVariance. |
| cv | Obtient ou définit une valeur de CV. |
| delay | Obtient ou définit une valeur de Delay. |
| finish | Obtient ou définit une valeur de Finish. |
| finish_variance | Obtient ou définit une valeur de FinishVariance. |
| hyperlink | Obtient ou définit une valeur de Hyperlink. |
| hyperlink_address | Obtient ou définit une valeur de HyperlinkAddress. |
| hyperlink_sub_address | Obtient ou définit une valeur de HyperlinkSubAddress. |
| work_variance | Obtient ou définit une valeur de WorkVariance. |
| has_fixed_rate_units | Obtient ou définit une valeur indiquant si HasFixedRateUnits est défini ou non. |
| fixed_material | Obtient ou définit une valeur indiquant si FixedMaterial est défini ou non. |
| leveling_delay | Obtient ou définit une valeur de LevelingDelay. |
| linked_fields | Obtient ou définit une valeur indiquant si LinkedFields est défini ou non. |
| milestone | Obtient ou définit une valeur indiquant si Milestone est défini ou non. |
| notes_text | Obtient ou définit le texte brut des notes extrait des données RTF. |
| notes_rtf | Obtient ou définit les notes texte au format RTF. |
| overallocated | Obtient ou définit une valeur indiquant si Overallocated est défini ou non. |
| overtime_cost | Obtient ou définit une valeur de OvertimeCost. |
| overtime_work | Obtient ou définit une valeur de OvertimeWork. |
| peak_units | Obtient ou définit une valeur de PeakUnits. |
| regular_work | Obtient ou définit une valeur de RegularWork. |
| remaining_cost | Obtient ou définit une valeur de RemainingCost. |
| remaining_overtime_cost | Obtient ou définit une valeur de RemainingOvertimeCost. |
| remaining_overtime_work | Obtient ou définit une valeur de RemainingOvertimeWork. |
| remaining_work | Obtient ou définit une valeur de RemainingWork. |
| response_pending | Obtient ou définit une valeur indiquant si ResponsePending est défini ou non. |
| start | Obtient ou définit une valeur de Start. |
| stop | Obtient ou définit une valeur de Stop. |
| resume | Obtient ou définit une valeur de Resume. |
| start_variance | Obtient ou définit une valeur de StartVariance. |
| summary | Obtient ou définit une valeur indiquant si Summary est défini ou non. |
| sv | Obtient ou définit une valeur de SV. |
| units | Obtient ou définit une valeur de Units. |
| update_needed | Obtient ou définit une valeur indiquant si UpdateNeeded est défini ou non. |
| vac | Obtient ou définit une valeur de VAC. |
| work | Obtient ou définit une valeur de Work. |
| work_contour | Obtient ou définit une valeur de WorkContour. |
| bcws | Obtient ou définit la valeur de BCWS. |
| bcwp | Obtient ou définit la valeur de BCWP. |
| booking_type | Obtient ou définit la valeur de BookingType. |
| actual_work_protected | Obtient ou définit une valeur de ActualWorkProtected. |
| actual_overtime_work_protected | Obtient ou définit une valeur de ActualOvertimeWorkProtected. |
| actual_overtime_work | Obtient ou définit une valeur de ActualOvertimeWork. |
| created | Obtient ou définit une valeur de Created. |
| assignment_owner | Obtient ou définit une valeur de AssignmentOwner. |
| assignment_owner_guid | Obtient ou définit une valeur de AssignmentOwnerGuid. |
| budget_cost | Obtient ou définit la valeur de BudgetCost. |
| budget_work | Obtient ou définit la valeur de BudgetWork. |
| rate_scale | Obtient ou définit une valeur de RateScale. |
| task | La tâche à laquelle une ressource est affectée. |
| resource | La ressource affectée à une tâche. |
| guid | Obtient ou définit l'identifiant unique pour cette affectation. |
| parent_project | Obtient le projet parent pour cette affectation. |
| baselines | Obtient l'objet AssignmentBaselineCollection.<br/>            La collection des valeurs de référence associées à une affectation. |
| extended_attributes | Obtient ou définit une instance de la classe ExtendedAttributeCollection pour cet objet. |
| timephased_data | Obtient ou définit l'instance de la classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenant des éléments de la classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/). |
## Méthodes
| Nom | Description |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | Renvoie l'instance de la classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenant des instances de la classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) dans les dates de début et de fin spécifiées du [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) donné. |
| get_timephased_data(start, end) | Renvoie l'instance de la classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenant des instances de la classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) dans les dates de début et de fin spécifiées du [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) donné. |
| get_timephased_work(start, end, timephased_data_type) | Obtient la quantité de travail phasé dans le temps pour l'intervalle de dates spécifié. |
| get_timephased_work(start, end) | Obtient la quantité de travail phasé dans le temps pour l'intervalle de dates spécifié. |
| delete() | Supprime l'affectation de ressources de la collection des affectations du projet. |
| equals(other) | Renvoie une valeur indiquant si cette instance est égale à une instance spécifiée de la classe [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/). |
| timephased_data_from_task_duration(calendar) | Génère une liste de données phasées dans le temps basée sur la durée de la tâche et la date de début planifiée. |
| make_t_ps(start, time, calendar, list, is_working, type) | Génère une liste de données phasées dans le temps. |
| split_task(start, finish, calendar) | Divise la tâche en deux parties. |
| set_material_resource_units(units, rate_scale_type) | Définit les unités pour l'affectation d'une ressource matérielle avec consommation variable de matériel.<br/>            La consommation variable de matériel signifie que, à mesure que la durée de l'affectation change, la quantité de matériaux utilisée change proportionnellement. |

### Voir aussi

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

