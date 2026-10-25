---
title: "ResourceAssignment"
second_title: "Aspose.Tasks för Python via .NET API-referens"
description: 
type: docs
weight: 980
url: /sv/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Representerar en resursallokering i ett projekt.

Typen ResourceAssignment visar följande medlemmar:
## Egenskaper
| Namn | Beskrivning |
| :- | :- |
| uid | Hämtar eller anger ett värde för Uid. |
| percent_work_complete | Hämtar eller anger ett värde för PercentWorkComplete. |
| actual_cost | Hämtar eller anger ett värde för ActualCost. |
| actual_finish | Hämtar eller anger ett värde för ActualFinish. |
| actual_overtime_cost | Hämtar eller anger ett värde för ActualOvertimeCost. |
| actual_start | Hämtar eller anger ett värde för ActualStart. |
| actual_work | Hämtar eller anger ett värde för ActualWork. |
| acwp | Hämtar eller anger ett värde för ACWP. |
| confirmed | Hämtar eller anger ett värde som indikerar om Confirmed är satt eller inte. |
| cost | Hämtar eller anger ett värde för Cost. |
| cost_rate_table_type | Hämtar eller anger ett värde för CostRateTableType. |
| cost_variance | Hämtar eller anger ett värde för CostVariance. |
| cv | Hämtar eller ange ett värde för CV. |
| delay | Hämtar eller anger ett värde för Delay. |
| finish | Hämtar eller ange ett värde för Finish. |
| finish_variance | Hämtar eller anger ett värde för FinishVariance. |
| hyperlink | Hämtar eller anger ett värde för Hyperlink. |
| hyperlink_address | Hämtar eller anger ett värde för HyperlinkAddress. |
| hyperlink_sub_address | Hämtar eller anger ett värde för HyperlinkSubAddress. |
| work_variance | Hämtar eller anger ett värde för WorkVariance. |
| has_fixed_rate_units | Hämtar eller anger ett värde som indikerar om HasFixedRateUnits är satt eller inte. |
| fixed_material | Hämtar eller anger ett värde som indikerar om FixedMaterial är satt eller inte. |
| leveling_delay | Hämtar eller anger ett värde för LevelingDelay. |
| linked_fields | Hämtar eller anger ett värde som indikerar om LinkedFields är satt eller inte. |
| milestone | Hämtar eller anger ett värde som indikerar om Milestone är satt eller inte. |
| notes_text | Hämtar eller anger noternas rentext som extraherats från RTF-data. |
| notes_rtf | Hämtar eller anger textnoterna i RTF-format. |
| overallocated | Hämtar eller anger ett värde som indikerar om Overallocated är angivet eller inte. |
| overtime_cost | Hämtar eller anger ett värde för OvertimeCost. |
| overtime_work | Hämtar eller anger ett värde för OvertimeWork. |
| peak_units | Hämtar eller anger ett värde för PeakUnits. |
| regular_work | Hämtar eller anger ett värde för RegularWork. |
| remaining_cost | Hämtar eller anger ett värde för RemainingCost. |
| remaining_overtime_cost | Hämtar eller anger ett värde för RemainingOvertimeCost. |
| remaining_overtime_work | Hämtar eller anger ett värde för RemainingOvertimeWork. |
| remaining_work | Hämtar eller anger ett värde för RemainingWork. |
| response_pending | Hämtar eller anger ett värde som indikerar om ResponsePending är satt eller inte. |
| start | Hämtar eller anger ett värde för Start. |
| stop | Hämtar eller anger ett värde för Stop. |
| resume | Hämtar eller anger ett värde för Resume. |
| start_variance | Hämtar eller anger ett värde för StartVariance. |
| summary | Hämtar eller anger ett värde som indikerar om Summary är satt eller inte. |
| sv | Hämtar eller anger ett värde för SV. |
| units | Hämtar eller anger ett värde för Units. |
| update_needed | Hämtar eller anger ett värde som indikerar om UpdateNeeded är satt eller inte. |
| vac | Hämtar eller anger ett värde för VAC. |
| work | Hämtar eller anger ett värde för Work. |
| work_contour | Hämtar eller anger ett värde för WorkContour. |
| bcws | Hämtar eller anger ett värde för BCWS. |
| bcwp | Hämtar eller anger ett värde för BCWP. |
| booking_type | Hämtar eller anger ett värde för BookingType. |
| actual_work_protected | Hämtar eller anger ett värde för ActualWorkProtected. |
| actual_overtime_work_protected | Hämtar eller anger ett värde för ActualOvertimeWorkProtected. |
| actual_overtime_work | Hämtar eller anger ett värde för ActualOvertimeWork. |
| created | Hämtar eller anger ett värde för Created. |
| assignment_owner | Hämtar eller anger ett värde för AssignmentOwner. |
| assignment_owner_guid | Hämtar eller anger ett värde för AssignmentOwnerGuid. |
| budget_cost | Hämtar eller anger ett värde för BudgetCost. |
| budget_work | Hämtar eller anger ett värde för BudgetWork. |
| rate_scale | Hämtar eller anger ett värde för RateScale. |
| task | Uppgiften som en resurs är tilldelad. |
| resource | Resursen som är tilldelad en uppgift. |
| guid | Hämtar eller anger ett unikt identifierare för denna tilldelning. |
| parent_project | Hämtar överordnat projekt för denna tilldelning. |
| baselines | Hämtar AssignmentBaselineCollection-objekt.<br/>            Samlingen av baslinjevärden som är kopplade till en tilldelning. |
| extended_attributes | Hämtar eller anger en instans av klassen ExtendedAttributeCollection för detta objekt. |
| timephased_data | Hämtar eller anger instansen av klassen [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) som innehåller element av klassen [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/). |
## Methods
| Namn | Beskrivning |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | Returnerar instansen av klassen [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) som innehåller instanser av klassen [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) inom angivna start- och slutdatum för den specificerade [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/). |
| get_timephased_data(start, end) | Returnerar instansen av klassen [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) som innehåller instanser av klassen [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) inom angivna start- och slutdatum för den specificerade [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/). |
| get_timephased_work(start, end, timephased_data_type) | Hämtar mängden tidsfasade arbete för det angivna datum- och tidsintervallet. |
| get_timephased_work(start, end) | Hämtar mängden tidsfasade arbete för det angivna datum- och tidsintervallet. |
| delete() | Tar bort resursens tilldelning från projektets tilldelningssamling. |
| equals(other) | Returnerar ett värde som indikerar om denna instans är lika med en specificerad instans av klassen [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/). |
| timephased_data_from_task_duration(calendar) | Genererar en lista med tidsfasade data baserat på uppgiftens varaktighet och det schemalagda startdatumet. |
| make_t_ps(start, time, calendar, list, is_working, type) | Genererar en lista med tidsfasade data. |
| split_task(start, finish, calendar) | Delar upp uppgiften i två delar. |
| set_material_resource_units(units, rate_scale_type) | Ställer in enheter för tilldelning av en materialresurs med variabel materialförbrukning.<br/>            Den variabla materialförbrukningen innebär att när tilldelningens varaktighet ändras, förändras mängden material som används proportionellt. |

### Se även

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

