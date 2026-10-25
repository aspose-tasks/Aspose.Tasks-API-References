---
title: "Aspose::Tasks::ExtendedAttributeDefinition класс"
linktitle: "ExtendedAttributeDefinition"
articleTitle: "ExtendedAttributeDefinition"
second_title: "Aspose.Tasks для C++"
description: "Представляет определение расширенного атрибута, связанное с проектом."
type: docs
weight: 10
url: /ru/cpp/aspose.tasks/extendedattributedefinition/
---

## ExtendedAttributeDefinition class

Представляет определение расширенного атрибута, связанное с проектом.

## Методы

| Имя | Описание |
| --- | --- |
| [AddLookupValue](./addlookupvalue/) | Добавляет значение во внутренний список поиска. Это предпочтительный способ работы со списком ValueList. |
| [CreateExtendedAttribute (7 overloads)](./createextendedattribute/) | Создаёт новый расширенный атрибут с идентификатором поля, который равен значению идентификатора поля этого объекта. |
| [CreateLookupResourceDefinition (2 overloads)](./createlookupresourcedefinition/) | Фабричный метод, который создаёт определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в ресурсах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода. |
| [CreateLookupTaskDefinition (2 overloads)](./createlookuptaskdefinition/) | Фабричный метод, который создаёт определение расширенного атрибута с поиском. Он имеет CalculationType, равный Tasks::CalculationType::Lookup, и может использоваться только в задачах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода. |
| [CreateResourceDefinition (2 overloads)](./createresourcedefinition/) | Фабричный метод, который создаёт простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в ресурсах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода. |
| [CreateTaskDefinition (2 overloads)](./createtaskdefinition/) | Фабричный метод, который создаёт простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет CalculationType, равный Tasks::CalculationType::None, и может использоваться только в задачах. Необходимо указать customFieldType, fieldId и alias при вызове этого метода. |
| [Equals](./equals/) | Возвращает флаг, указывающий, равен ли данный экземпляр указанному объекту. |
| [get_Alias](./get_alias/) | Получает псевдоним пользовательского поля. |
| [get_AppendNewValues](./get_appendnewvalues/) | Получает значение, указывающее, добавляются ли новые значения, добавленные в проект, автоматически в список. |
| [get_AutoRollDown](./get_autorolldown/) | Получает значение, указывающее, включено ли автоматическое распространение на назначения. |
| [get_CalculationType](./get_calculationtype/) | Получает тип расчёта значения пользовательского атрибута. |
| [get_CfType](./get_cftype/) | Получает тип пользовательского поля. |
| [get_Default](./get_default/) | Получает значение по умолчанию в списке. |
| [get_DefaultGuid](./get_defaultguid/) | Получает Guid записи таблицы поиска по умолчанию. |
| [get_ElementType](./get_elementtype/) | Получает, связан ли расширенный атрибут с задачей, ресурсом или назначением. |
| [get_FieldId](./get_fieldid/) | Получает значение, соответствующее идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса Aspose::Tasks::ExtendedAttributeTask для указания свойства FieldId. |
| [get_FieldName](./get_fieldname/) | Получает имя пользовательского поля. |
| [get_Formula](./get_formula/) | Получает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи. |
| [get_GraphicalIndicator](./get_graphicalindicator/) | Получает информацию о графических индикаторах, связанных с расширенным атрибутом. Применимо к формату MPP. |
| [get_Guid](./get_guid/) | Получает Guid пользовательского поля. |
| [get_LookupUid](./get_lookupuid/) | Получает Guid таблицы поиска, связанной с пользовательским полем. |
| [get_MaxMultiValues](./get_maxmultivalues/) | Получает максимальное количество значений, которое можно установить в выпадающем списке. |
| [get_ParentProject](./get_parentproject/) | Получает родительский проект для экземпляра ExtendedAttributeDefinition. |
| [get_PhoneticsAlias](./get_phoneticsalias/) | Получает фонетическое произношение псевдонима пользовательского поля. |
| [get_RestrictValues](./get_restrictvalues/) | Получает значение, указывающее, ограничены ли значения пользовательского поля значениями из ValueList. |
| [get_RollupType](./get_rolluptype/) | Получает способ расчёта агрегированных значений. |
| [get_SecondaryGuid](./get_secondaryguid/) | Получает вторичный guid расширенного атрибута. |
| [get_SecondaryPid](./get_secondarypid/) | Получает вторичный PID пользовательского поля. |
| [get_SummaryRowsCalculationType](./get_summaryrowscalculationtype/) | Получает тип расчёта значения пользовательского атрибута для строк‑итогов. |
| [get_UserDef](./get_userdef/) | Получает значение, указывающее, является ли пользовательское поле определённым пользователем. |
| [get_ValueList](./get_valuelist/) | Получает List< Value > ValueList. |
| [get_ValuelistSortOrder](./get_valuelistsortorder/) | Получает способ сортировки списков значений. Значения: 0=По убыванию, 1=По возрастанию. |
| [GetHashCode](./gethashcode/) | Возвращает хеш‑код для экземпляра класса ExtendedAttributeDefinition. |
| [RemoveLookupValue](./removelookupvalue/) | Удаляет значение из внутреннего списка поиска. Это предпочтительный способ манипуляций со списком ValueList. |
| [set_Alias](./set_alias/) | Устанавливает псевдоним пользовательского поля. |
| [set_AppendNewValues](./set_appendnewvalues/) | Устанавливает значение, указывающее, добавляются ли новые значения, внесённые в проект, автоматически в список. |
| [set_AutoRollDown](./set_autorolldown/) | Устанавливает значение, указывающее, включено ли автоматическое распространение на назначения. |
| [set_CalculationType](./set_calculationtype/) | Устанавливает тип расчёта значения пользовательского атрибута. |
| [set_Default](./set_default/) | Устанавливает значение по умолчанию в списке. |
| [set_DefaultGuid](./set_defaultguid/) | Устанавливает Guid записи таблицы поиска по умолчанию. |
| [set_ElementType](./set_elementtype/) | Устанавливает, связан ли расширенный атрибут с задачей, ресурсом или назначением. |
| [set_FieldId](./set_fieldid/) | Устанавливает соответствие идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса Aspose::Tasks::ExtendedAttributeTask для указания свойства FieldId. |
| [set_Formula](./set_formula/) | Устанавливает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи. |
| [set_GraphicalIndicator](./set_graphicalindicator/) | Устанавливает информацию о графических индикаторах, связанную с расширенным атрибутом. Применимо к формату MPP. |
| [set_Guid](./set_guid/) | Устанавливает Guid пользовательского поля. |
| [set_MaxMultiValues](./set_maxmultivalues/) | Устанавливает максимальное количество значений, которое можно задать в выпадающем списке. |
| [set_PhoneticsAlias](./set_phoneticsalias/) | Устанавливает фонетическое произношение псевдонима пользовательского поля. |
| [set_RestrictValues](./set_restrictvalues/) | Устанавливает значение, указывающее, ограничены ли значения пользовательского поля значениями из списка ValueList. |
| [set_RollupType](./set_rolluptype/) | Устанавливает способ расчёта сводных данных. |
| [set_SecondaryGuid](./set_secondaryguid/) | Устанавливает вторичный guid расширенного атрибута. |
| [set_SecondaryPid](./set_secondarypid/) | Устанавливает вторичный PID пользовательского поля. |
| [set_SummaryRowsCalculationType](./set_summaryrowscalculationtype/) | Устанавливает тип расчёта значения пользовательского атрибута для строк‑итогов. |
| [set_UserDef](./set_userdef/) | Устанавливает значение, указывающее, определено ли пользовательское поле пользователем. |
| [set_ValuelistSortOrder](./set_valuelistsortorder/) | Устанавливает способ сортировки списков значений. Значения: 0=по убыванию, 1=по возрастанию. |

