---
title: "ExtendedAttributeDefinition"
second_title: "Справочник API Aspose.Tasks для Python через .NET"
description: 
type: docs
weight: 310
url: /ru/python-net/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Представляет определение расширенного атрибута, связанного с проектом.

Тип ExtendedAttributeDefinition раскрывает следующие члены:
## Свойства
| Имя | Описание |
| :- | :- |
| field_id | Получает или задает значение, соответствующее идентификатору проекта пользовательского поля.<br/>            Используйте строковое представление константы из класса [ExtendedAttributeTask](/tasks/python-net/aspose.tasks/extendedattributetask/) для указания свойства [field_id](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| field_name | Получает имя пользовательского поля. |
| cf_type | Получает тип пользовательского поля. |
| guid | Получает или задает GUID пользовательского поля. |
| element_type | Получает или задает расширенный атрибут, связанный<br/>            с задачей, ресурсом или назначением. |
| max_multi_values | Получает или задает максимальное количество значений, которое можно установить в списке выбора. |
| user_def | Получает или задает значение, указывающее, является ли пользовательское поле определённым пользователем. |
| alias | Получает или задает псевдоним пользовательского поля. |
| secondary_pid | Получает или задает вторичный PID пользовательского поля. |
| auto_roll_down | Получает или задает значение, указывающее, включено ли автоматическое раскрытие до назначений. |
| default_guid | Получает или задает Guid записи таблицы поиска по умолчанию. |
| lookup_uid | Получает Guid таблицы поиска, связанной с пользовательским полем. |
| phonetics_alias | Получает или задает фонетическое произношение псевдонима пользовательского поля. |
| rollup_type | Получает или задает способ расчёта сводных данных. |
| calculation_type | Получает или задает тип расчёта значения пользовательского атрибута. |
| summary_rows_calculation_type | Получает или задает тип расчёта значения пользовательского атрибута для строк сводки. |
| formula | Получает или задает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи. |
| graphical_indicator | Получает или задает информацию о графических индикаторах, связанную с расширенным атрибутом.<br/>            Применимо к формату MPP. |
| restrict_values | Получает или задает значение, указывающее, ограничены ли значения пользовательского поля значениями из [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| valuelist_sort_order | Получает или задает способ сортировки списков значений. Значения: 0=По убыванию, 1=По возрастанию. |
| append_new_values | Получает или задает значение, указывающее, добавляются ли новые значения, внесённые в проект, автоматически в список. |
| default | Получает или задает значение по умолчанию в списке. |
| value_list | Получает List<Value> ValueList. |
| secondary_guid | Получает или задает вторичный guid расширенного атрибута. |
| parent_project | Получает родительский проект для экземпляра [ExtendedAttributeDefinition](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
## Методы
| Имя | Описание |
| :- | :- |
| create_extended_attribute() | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта. |
| create_extended_attribute(text_value) | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным текстовым значением. |
| create_extended_attribute(numeric_value) | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным числовым значением. |
| create_extended_attribute(date_time_value) | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением даты. |
| create_extended_attribute(duration_value) | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением длительности. |
| create_extended_attribute(flag_value) | Создаёт новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным флаговым значением. |
| create_extended_attribute(lookup_value) | Создает новый расширенный атрибут, связанный с указанным элементом [Value](/tasks/python-net/aspose.tasks/value/). |
| create_task_definition(custom_field_type, field_id, alias) | Фабричный метод, создающий простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\".<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [NONE](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Tasks.<br/>            Требуется указать |
| create_task_definition(field_id, alias) | Фабричный метод, создающий простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\".<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [NONE](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Tasks.<br/>            Требуется указать |
| create_resource_definition(custom_field_type, field_id, alias) | Фабричный метод, создающий простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\".<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [NONE](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Resource.<br/>            Требуется указать |
| create_resource_definition(field_id, alias) | Фабричный метод, создающий простое определение расширенного атрибута, которое Microsoft Project отображает как \"None\".<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [NONE](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Resource.<br/>            Требуется указать |
| create_lookup_task_definition(field_id, alias) | Фабричный метод, создающий определение расширенного атрибута с lookup.<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Tasks.<br/>            Требуется указать |
| create_lookup_task_definition(custom_field_type, field_id, alias) | Фабричный метод, создающий определение расширенного атрибута с lookup.<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Tasks.<br/>            Требуется указать |
| create_lookup_resource_definition(field_id, alias) | Фабричный метод, создающий определение расширенного атрибута с lookup.<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Resources.<br/>            Требуется указать |
| create_lookup_resource_definition(custom_field_type, field_id, alias) | Фабричный метод, создающий определение расширенного атрибута с lookup.<br/>            Он имеет [calculation_type](/tasks/python-net/aspose.tasks/extendedattributedefinition/) равный [LOOKUP](/tasks/python-net/aspose.tasks/calculationtype/) и может использоваться только в Resources.<br/>            Требуется указать |
| add_lookup_value(value) | Добавляет значение во внутренний список поиска. Это предпочтительный способ работы со [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |
| remove_lookup_value(value) | Удаляет значение из внутреннего списка поиска. Это предпочтительный способ работы со [value_list](/tasks/python-net/aspose.tasks/extendedattributedefinition/). |

### См. также

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

