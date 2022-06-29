---
title: ExtendedAttributeDefinition
second_title: Справочник по Aspose.Tasks для .NET API
description: Представляет расширенное определение атрибута связанное с проектом.
type: docs
weight: 530
url: /ru/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Представляет расширенное определение атрибута, связанное с проектом.

```csharp
public class ExtendedAttributeDefinition
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias) { get; set; } | Получает или задает псевдоним настраиваемого поля. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues) { get; set; } | Получает или задает значение, указывающее, добавляются ли новые значения, добавленные в проект, в список автоматически. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown) { get; set; } | Получает или задает значение, указывающее, включен ли автоматический переход к назначениям. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype) { get; set; } | Получает или задает тип расчета значения пользовательского атрибута. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype) { get; } | Получает тип настраиваемого поля. |
| [Default](../../aspose.tasks/extendedattributedefinition/default) { get; set; } | Получает или задает значение по умолчанию в списке. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid) { get; set; } | Получает или задает Guid записи таблицы поиска по умолчанию. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype) { get; set; } | Получает или устанавливает расширенный атрибут, связанный с задачей, ресурсом или заданием. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid) { get; set; } | Получает или устанавливает соответствие идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса[`ExtendedAttributeTask`](../extendedattributetask)для указания свойства[`FieldId`](./fieldid). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname) { get; } | Получает имя пользовательского поля. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula) { get; set; } | Получает или задает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid) { get; set; } | Получает или задает Guid пользовательского поля. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid) { get; } | Получает Guid таблицы поиска, связанной с настраиваемым полем. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues) { get; set; } | Получает или задает максимальное количество значений, которое можно задать в списке выбора. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject) { get; } | Получает родительский проект для экземпляра[`ExtendedAttributeDefinition`](../extendedattributedefinition). |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias) { get; set; } | Получает или задает фонетическое произношение псевдонима настраиваемого поля. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues) { get; set; } | Получает или задает значение, указывающее, ограничены ли значения настраиваемого поля значениями в[`ValueList`](./valuelist). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype) { get; set; } | Получает или задает способ расчета сводок. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid) { get; set; } | Получает или задает дополнительный идентификатор расширенного атрибута. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid) { get; set; } | Получает или задает вторичный PID пользовательского поля. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype) { get; set; } | Получает или задает тип расчета значения пользовательского атрибута для строк сводки. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef) { get; set; } | Получает или задает значение, указывающее, определено ли пользовательское поле пользователем. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist) { get; } | Получает список&lt;Value&gt; Список значений. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder) { get; set; } | Получает или задает способ сортировки списков значений. Значения:0=По убыванию, 1=По возрастанию. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Фабричный метод, создающий расширенное определение атрибута с поиском. Он имеет[`CalculationType`](./calculationtype)равноLookupи может использоваться в Только ресурсы. Вы должны указать*fieldId*и*alias*при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Фабричный метод, создающий расширенное определение атрибута с поиском. Он имеет[`CalculationType`](./calculationtype)равноLookupи может использоваться в Только ресурсы. Вы должны указать*customFieldType*,*fieldId*и*alias*при вызове этого метода. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Фабричный метод, создающий расширенное определение атрибута с поиском. Он имеет[`CalculationType`](./calculationtype)равноLookupи может использоваться в Только задачи. Вы должны указать*fieldId*и*alias*при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Фабричный метод, создающий расширенное определение атрибута с поиском. Он имеет[`CalculationType`](./calculationtype)равноLookupи может использоваться в Только задачи. Вы должны указать*customFieldType*,*fieldId*и*alias*при вызове этого метода. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition_1)(ExtendedAttributeResource, string) | Фабричный метод, который создает простое расширенное определение атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](./calculationtype)равноNoneи может использоваться в Только ресурс. Вы должны указать*fieldId*и*alias*при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Фабричный метод, который создает простое расширенное определение атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](./calculationtype)равноNoneи может использоваться в Только ресурс. Вы должны указать*customFieldType*,*fieldId*и*alias*при вызове этого метода. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition_1)(ExtendedAttributeTask, string) | Фабричный метод, который создает простое расширенное определение атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](./calculationtype)равноNoneи может использоваться в Только задачи. Вы должны указать*fieldId*и*alias*при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Фабричный метод, который создает простое расширенное определение атрибута, которое Microsoft Project показывает как «Нет». Он имеет[`CalculationType`](./calculationtype)равноNoneи может использоваться в Только задачи. Вы должны указать*customFieldType*,*fieldId*и*alias*при вызове этого метода. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue)(Value) | Добавляет значение во внутренний список поиска. Это предпочтительный способ для манипуляций с[`ValueList`](./valuelist). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute)() | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_3)(bool) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта и указанному значению флага. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_4)(DateTime) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта и указанному значению даты. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_5)(decimal) | Создает новый расширенный атрибут с идентификатором поля, который равен значению идентификатора поля этого объекта и указанному числовому значению. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_1)(Duration) | Создает новый расширенный атрибут с идентификатором поля, который равен значению идентификатора поля этого объекта и указанному значению продолжительности. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_6)(string) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта и указанному текстовому значению. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute#createextendedattribute_2)(Value) | Создает новый расширенный атрибут, связанный с указанным[`Value`](../value)элементом. |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals)(object) | Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode)() | Возвращает хэш-код экземпляра класса[`ExtendedAttributeDefinition`](../extendedattributedefinition). |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue)(Value) | Удаляет значение из внутреннего списка поиска. Это предпочтительный способ для манипуляций с[`ValueList`](./valuelist). |

### Смотрите также

* пространство имен [Aspose.Tasks](../../aspose.tasks)
* сборка [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
