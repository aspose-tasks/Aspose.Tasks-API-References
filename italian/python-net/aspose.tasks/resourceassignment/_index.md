---
title: "ResourceAssignment"
second_title: "Riferimento API di Aspose.Tasks per Python via .NET"
description: 
type: docs
weight: 980
url: /it/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Rappresenta un'assegnazione di risorsa in un progetto.

Il tipo ResourceAssignment espone i seguenti membri:
## Proprietà
| Nome | Descrizione |
| :- | :- |
| uid | Ottiene o imposta un valore di Uid. |
| percent_work_complete | Ottiene o imposta un valore di PercentWorkComplete. |
| actual_cost | Ottiene o imposta un valore di ActualCost. |
| actual_finish | Ottiene o imposta un valore di ActualFinish. |
| actual_overtime_cost | Ottiene o imposta un valore di ActualOvertimeCost. |
| actual_start | Ottiene o imposta un valore di ActualStart. |
| actual_work | Ottiene o imposta un valore di ActualWork. |
| acwp | Ottiene o imposta un valore di ACWP. |
| confirmed | Ottiene o imposta un valore che indica se Confirmed è impostato o meno. |
| cost | Ottiene o imposta un valore di Cost. |
| cost_rate_table_type | Ottiene o imposta un valore di CostRateTableType. |
| cost_variance | Ottiene o imposta un valore di CostVariance. |
| cv | Ottiene o imposta un valore di CV. |
| delay | Ottiene o imposta un valore di Delay. |
| finish | Ottiene o imposta un valore di Finish. |
| finish_variance | Ottiene o imposta un valore di FinishVariance. |
| hyperlink | Ottiene o imposta un valore di Hyperlink. |
| hyperlink_address | Ottiene o imposta un valore di HyperlinkAddress. |
| hyperlink_sub_address | Ottiene o imposta un valore di HyperlinkSubAddress. |
| work_variance | Ottiene o imposta un valore di WorkVariance. |
| has_fixed_rate_units | Ottiene o imposta un valore che indica se HasFixedRateUnits è impostato o meno. |
| fixed_material | Ottiene o imposta un valore che indica se FixedMaterial è impostato o meno. |
| leveling_delay | Ottiene o imposta un valore di LevelingDelay. |
| linked_fields | Ottiene o imposta un valore che indica se LinkedFields è impostato o meno. |
| milestone | Ottiene o imposta un valore che indica se Milestone è impostato o meno. |
| notes_text | Ottiene o imposta il testo semplice delle note estratto dai dati RTF. |
| notes_rtf | Ottiene o imposta le note di testo in formato RTF. |
| overallocated | Ottiene o imposta un valore che indica se Overallocated è impostato o meno. |
| overtime_cost | Ottiene o imposta un valore di OvertimeCost. |
| overtime_work | Ottiene o imposta un valore di OvertimeWork. |
| peak_units | Ottiene o imposta un valore di PeakUnits. |
| regular_work | Ottiene o imposta un valore di RegularWork. |
| remaining_cost | Ottiene o imposta un valore di RemainingCost. |
| remaining_overtime_cost | Ottiene o imposta un valore di RemainingOvertimeCost. |
| remaining_overtime_work | Ottiene o imposta un valore di RemainingOvertimeWork. |
| remaining_work | Ottiene o imposta un valore di RemainingWork. |
| response_pending | Ottiene o imposta un valore che indica se ResponsePending è impostato o meno. |
| avvio | Ottiene o imposta un valore di Start. |
| stop | Ottiene o imposta un valore di Stop. |
| resume | Ottiene o imposta un valore di Resume. |
| start_variance | Ottiene o imposta un valore di StartVariance. |
| summary | Ottiene o imposta un valore che indica se Summary è impostato o meno. |
| sv | Ottiene o imposta un valore di SV. |
| units | Ottiene o imposta un valore di Units. |
| update_needed | Ottiene o imposta un valore che indica se UpdateNeeded è impostato o meno. |
| vac | Ottiene o imposta un valore di VAC. |
| lavoro | Ottiene o imposta un valore di Work. |
| work_contour | Ottiene o imposta un valore di WorkContour. |
| bcws | Ottiene o imposta un valore di BCWS. |
| bcwp | Ottiene o imposta un valore di BCWP. |
| booking_type | Ottiene o imposta un valore di BookingType. |
| actual_work_protected | Ottiene o imposta un valore di ActualWorkProtected. |
| actual_overtime_work_protected | Ottiene o imposta un valore di ActualOvertimeWorkProtected. |
| actual_overtime_work | Ottiene o imposta un valore di ActualOvertimeWork. |
| created | Ottiene o imposta un valore di Created. |
| assignment_owner | Ottiene o imposta un valore di AssignmentOwner. |
| assignment_owner_guid | Ottiene o imposta un valore di AssignmentOwnerGuid. |
| budget_cost | Ottiene o imposta un valore di BudgetCost. |
| budget_work | Ottiene o imposta un valore di BudgetWork. |
| rate_scale | Ottiene o imposta un valore di RateScale. |
| task | L'attività a cui è assegnata una risorsa. |
| resource | La risorsa assegnata a un'attività. |
| guid | Ottiene o imposta l'identificatore univoco per questa assegnazione. |
| parent_project | Ottiene il progetto padre per questa assegnazione. |
| baselines | Ottiene l'oggetto AssignmentBaselineCollection.<br/>            La raccolta dei valori di baseline associati a un'assegnazione. |
| extended_attributes | Ottiene o imposta un'istanza della classe ExtendedAttributeCollection per questo oggetto. |
| timephased_data | Ottiene o imposta l'istanza della classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenente elementi della classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/). |
## Methods
| Nome | Descrizione |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | Restituisce l'istanza della classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenente istanze della classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) entro le date di inizio e fine specificate per il [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) indicato. |
| get_timephased_data(start, end) | Restituisce l'istanza della classe [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) contenente istanze della classe [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) entro le date di inizio e fine specificate per il [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) indicato. |
| get_timephased_work(start, end, timephased_data_type) | Ottiene la quantità di lavoro timephased per l'intervallo di data/ora specificato. |
| get_timephased_work(start, end) | Ottiene la quantità di lavoro timephased per l'intervallo di data/ora specificato. |
| delete() | Elimina l'assegnazione di risorsa dalla raccolta delle assegnazioni del progetto. |
| equals(other) | Restituisce un valore che indica se questa istanza è uguale a una specifica istanza della classe [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/). |
| timephased_data_from_task_duration(calendar) | Genera un elenco di dati timephased basato sulla durata dell'attività e sulla data di inizio programmata. |
| make_t_ps(start, time, calendar, list, is_working, type) | Genera un elenco di dati timephased. |
| split_task(start, finish, calendar) | Divide l'attività in due parti. |
| set_material_resource_units(units, rate_scale_type) | Imposta le unità per l'assegnazione di una risorsa materiale con consumo variabile di materiale.<br/>            Il consumo variabile di materiale significa che, al variare della durata dell'assegnazione, la quantità di materiali utilizzati cambia proporzionalmente. |

### Vedi anche

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

