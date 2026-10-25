---
title: "ResourceAssignment"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 980
url: /ru/python-net/aspose.tasks/resourceassignment/
---

## ResourceAssignment class

Представляет назначение ресурса в проекте.

Тип ResourceAssignment раскрывает следующие члены:
## Свойства
| Имя | Описание |
| :- | :- |
| uid | Получает или задает значение свойства Uid. |
| percent_work_complete | Получает или задает значение PercentWorkComplete. |
| actual_cost | Получает или задает значение ActualCost. |
| actual_finish | Получает или задает значение ActualFinish. |
| actual_overtime_cost | Получает или задает значение ActualOvertimeCost. |
| actual_start | Получает или задает значение ActualStart. |
| actual_work | Получает или задает значение ActualWork. |
| acwp | Получает или задает значение ACWP. |
| confirmed | Получает или задает значение, указывающее, установлено ли Confirmed или нет. |
| cost | Получает или задает значение Cost. |
| cost_rate_table_type | Получает или задает значение CostRateTableType. |
| cost_variance | Получает или задает значение CostVariance. |
| cv | Получает или задает значение CV. |
| delay | Получает или задает значение Delay. |
| finish | Получает или задает значение Finish. |
| finish_variance | Получает или задает значение FinishVariance. |
| hyperlink | Получает или задает значение Hyperlink. |
| hyperlink_address | Получает или задает значение HyperlinkAddress. |
| hyperlink_sub_address | Получает или задает значение HyperlinkSubAddress. |
| work_variance | Получает или задает значение свойства WorkVariance. |
| has_fixed_rate_units | Получает или задает значение, указывающее, установлено ли HasFixedRateUnits или нет. |
| fixed_material | Получает или задает значение, указывающее, установлено ли FixedMaterial или нет. |
| leveling_delay | Получает или задает значение LevelingDelay. |
| linked_fields | Получает или задает значение, указывающее, установлено ли LinkedFields или нет. |
| milestone | Получает или задает значение, указывающее, установлено ли Milestone или нет. |
| notes_text | Получает или задает обычный текст заметок, извлеченный из данных RTF. |
| notes_rtf | Получает или задает текстовые заметки в формате RTF. |
| overallocated | Получает или задает значение, указывающее, установлен ли Overallocated, или нет. |
| overtime_cost | Получает или задает значение OvertimeCost. |
| overtime_work | Получает или задает значение OvertimeWork. |
| peak_units | Получает или задает значение PeakUnits. |
| regular_work | Получает или задает значение RegularWork. |
| remaining_cost | Получает или задает значение RemainingCost. |
| remaining_overtime_cost | Получает или задает значение RemainingOvertimeCost. |
| remaining_overtime_work | Получает или задает значение RemainingOvertimeWork. |
| remaining_work | Получает или задает значение RemainingWork. |
| response_pending | Получает или задает значение, указывающее, установлено ли ResponsePending. |
| начало | Получает или задает значение свойства Start. |
| stop | Получает или задает значение Stop. |
| resume | Получает или задает значение Resume. |
| start_variance | Получает или задает значение StartVariance. |
| summary | Получает или задает значение, указывающее, установлено ли Summary. |
| sv | Получает или задает значение свойства SV. |
| units | Получает или задает значение Units. |
| update_needed | Получает или задает значение, указывающее, установлено ли UpdateNeeded. |
| vac | Получает или задает значение VAC. |
| work | Получает или задает значение свойства Work. |
| work_contour | Получает или задает значение WorkContour. |
| bcws | Получает или задает значение BCWS. |
| bcwp | Получает или задает значение BCWP. |
| booking_type | Получает или задает значение BookingType. |
| actual_work_protected | Получает или задает значение ActualWorkProtected. |
| actual_overtime_work_protected | Получает или задает значение ActualOvertimeWorkProtected. |
| actual_overtime_work | Получает или задает значение ActualOvertimeWork. |
| created | Получает или задает значение Created. |
| assignment_owner | Получает или задает значение AssignmentOwner. |
| assignment_owner_guid | Получает или задает значение AssignmentOwnerGuid. |
| budget_cost | Получает или задает значение BudgetCost. |
| budget_work | Получает или задает значение BudgetWork. |
| rate_scale | Получает или задает значение RateScale. |
| task | Задача, к которой назначен ресурс. |
| resource | Ресурс, назначенный задаче. |
| guid | Получает или задает уникальный идентификатор для этого назначения. |
| parent_project | Получает родительский проект для этого назначения. |
| baselines | Получает объект AssignmentBaselineCollection.<br/>            Коллекция базовых значений, связанных с назначением. |
| extended_attributes | Получает или задает экземпляр класса ExtendedAttributeCollection для этого объекта. |
| timephased_data | Получает или задает экземпляр класса [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/), содержащий элементы класса [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/). |
## Методы
| Имя | Описание |
| :- | :- |
| get_timephased_data(start, end, timephased_type) | Возвращает экземпляр класса [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/), содержащий экземпляры класса [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) в указанных датах начала и окончания заданного [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/). |
| get_timephased_data(start, end) | Возвращает экземпляр класса [TimephasedDataCollection](/tasks/python-net/aspose.tasks/timephaseddatacollection/), содержащий экземпляры класса [timephased_data](/tasks/python-net/aspose.tasks/resourceassignment/) в указанных датах начала и окончания заданного [TimephasedDataType](/tasks/python-net/aspose.tasks/timephaseddatatype/). |
| get_timephased_work(start, end, timephased_data_type) | Получает количество timephased work для указанного интервала дат и времени. |
| get_timephased_work(start, end) | Получает количество timephased work для указанного интервала дат и времени. |
| delete() | Удаляет назначение ресурса из коллекции назначений проекта. |
| equals(other) | Возвращает значение, указывающее, равен ли данный экземпляр указанному экземпляру класса [ResourceAssignment](/tasks/python-net/aspose.tasks/resourceassignment/). |
| timephased_data_from_task_duration(calendar) | Генерирует список фазовых данных на основе длительности задачи и запланированной даты начала. |
| make_t_ps(start, time, calendar, list, is_working, type) | Генерирует список фазовых данных. |
| split_task(start, finish, calendar) | Разделяет задачу на две части. |
| set_material_resource_units(units, rate_scale_type) | Устанавливает единицы измерения для назначения материального ресурса с переменным потреблением материалов.<br/>            Переменное потребление материалов означает, что при изменении длительности назначения количество используемых материалов меняется пропорционально. |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

