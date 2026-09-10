---
title: "ResourceAssignment"
second_title: "Referencia de API de Aspose.Tasks para Python vía .NET"
description: 
type: docs
weight: 980
url: /es/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Representa una asignación de recurso en un proyecto.

El tipo ResourceAssignment expone los siguientes miembros:
## Propiedades
| Nombre | Descripción |
| :- | :- |
| uid | Obtiene o establece un valor de Uid. |
| percent_work_complete | Obtiene o establece un valor de PercentWorkComplete. |
| actual_cost | Obtiene o establece un valor de ActualCost. |
| actual_finish | Obtiene o establece un valor de ActualFinish. |
| actual_overtime_cost | Obtiene o establece un valor de ActualOvertimeCost. |
| actual_start | Obtiene o establece un valor de ActualStart. |
| actual_work | Obtiene o establece un valor de ActualWork. |
| acwp | Obtiene o establece un valor de ACWP. |
| confirmed | Obtiene o establece un valor que indica si Confirmed está establecido o no. |
| cost | Obtiene o establece un valor de Cost. |
| cost_rate_table_type | Obtiene o establece un valor de CostRateTableType. |
| cost_variance | Obtiene o establece un valor de CostVariance. |
| cv | Obtiene o establece un valor de CV. |
| delay | Obtiene o establece un valor de Delay. |
| finish | Obtiene o establece un valor de Finish. |
| finish_variance | Obtiene o establece un valor de FinishVariance. |
| hyperlink | Obtiene o establece un valor de Hyperlink. |
| hyperlink_address | Obtiene o establece un valor de HyperlinkAddress. |
| hyperlink_sub_address | Obtiene o establece un valor de HyperlinkSubAddress. |
| work_variance | Obtiene o establece un valor de WorkVariance. |
| has_fixed_rate_units | Obtiene o establece un valor que indica si HasFixedRateUnits está establecido o no. |
| fixed_material | Obtiene o establece un valor que indica si FixedMaterial está establecido o no. |
| leveling_delay | Obtiene o establece un valor de LevelingDelay. |
| linked_fields | Obtiene o establece un valor que indica si LinkedFields está establecido o no. |
| milestone | Obtiene o establece un valor que indica si Milestone está establecido o no. |
| notes_text | Obtiene o establece el texto sin formato de las notas extraído de datos RTF. |
| notes_rtf | Obtiene o establece las notas de texto en formato RTF. |
| overallocated | Obtiene o establece un valor que indica si Overallocated está establecido o no. |
| overtime_cost | Obtiene o establece un valor de OvertimeCost. |
| overtime_work | Obtiene o establece un valor de OvertimeWork. |
| peak_units | Obtiene o establece un valor de PeakUnits. |
| regular_work | Obtiene o establece un valor de RegularWork. |
| remaining_cost | Obtiene o establece un valor de RemainingCost. |
| remaining_overtime_cost | Obtiene o establece un valor de RemainingOvertimeCost. |
| remaining_overtime_work | Obtiene o establece un valor de RemainingOvertimeWork. |
| remaining_work | Obtiene o establece un valor de RemainingWork. |
| response_pending | Obtiene o establece un valor que indica si ResponsePending está establecido o no. |
| inicio | Obtiene o establece un valor de Start. |
| stop | Obtiene o establece un valor de Stop. |
| resume | Obtiene o establece un valor de Resume. |
| start_variance | Obtiene o establece un valor de StartVariance. |
| summary | Obtiene o establece un valor que indica si Summary está establecido o no. |
| sv | Obtiene o establece un valor de SV. |
| units | Obtiene o establece un valor de Units. |
| update_needed | Obtiene o establece un valor que indica si UpdateNeeded está establecido o no. |
| vac | Obtiene o establece un valor de VAC. |
| work | Obtiene o establece un valor de Work. |
| work_contour | Obtiene o establece un valor de WorkContour. |
| bcws | Obtiene o establece un valor de BCWS. |
| bcwp | Obtiene o establece un valor de BCWP. |
| booking_type | Obtiene o establece un valor de BookingType. |
| actual_work_protected | Obtiene o establece un valor de ActualWorkProtected. |
| actual_overtime_work_protected | Obtiene o establece un valor de ActualOvertimeWorkProtected. |
| actual_overtime_work | Obtiene o establece un valor de ActualOvertimeWork. |
| created | Obtiene o establece un valor de Created. |
| assignment_owner | Obtiene o establece un valor de AssignmentOwner. |
| assignment_owner_guid | Obtiene o establece un valor de AssignmentOwnerGuid. |
| budget_cost | Obtiene o establece un valor de BudgetCost. |
| budget_work | Obtiene o establece un valor de BudgetWork. |
| rate_scale | Obtiene o establece un valor de RateScale. |
| task | La tarea a la que se asigna un recurso. |
| resource | El recurso asignado a una tarea. |
| guid | Obtiene o establece el identificador único para esta asignación. |
| parent_project | Obtiene el proyecto principal para esta asignación. |
| baselines | Obtiene el objeto AssignmentBaselineCollection.<br/>            La colección de valores de línea base asociados a una asignación. |
| extended_attributes | Obtiene o establece una instancia de la clase ExtendedAttributeCollection para este objeto. |
| timephased_data | Obtiene o establece la instancia de la clase [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) que contiene elementos de la clase [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/). |
## Métodos
| Nombre | Descripción |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | Devuelve la instancia de la clase [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) que contiene instancias de la clase [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) dentro de las fechas de inicio y fin especificadas del [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) indicado. |
| get_timephased_data(start, end) | Devuelve la instancia de la clase [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/) que contiene instancias de la clase [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) dentro de las fechas de inicio y fin especificadas del [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/) indicado. |
| get_timephased_work(start, end, timephased_data_type) | Obtiene la cantidad de trabajo timephased para el intervalo de fecha y hora especificado. |
| get_timephased_work(start, end) | Obtiene la cantidad de trabajo timephased para el intervalo de fecha y hora especificado. |
| delete() | Elimina la asignación de recursos de la colección de asignaciones del proyecto. |
| equals(other) | Devuelve un valor que indica si esta instancia es igual a una instancia especificada de la clase [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/). |
| timephased_data_from_task_duration(calendar) | Genera una lista de datos faseados en función de la duración de la tarea y la fecha de inicio programada. |
| make_t_ps(start, time, calendar, list, is_working, type) | Genera una lista de datos faseados. |
| split_task(start, finish, calendar) | Divide la tarea en dos partes. |
| set_material_resource_units(units, rate_scale_type) | Establece unidades para la asignación de un recurso material con consumo de material variable.<br/>            El consumo de material variable significa que, a medida que cambia la duración de la asignación, la cantidad de materiales utilizados cambia proporcionalmente. |

### Ver también

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

