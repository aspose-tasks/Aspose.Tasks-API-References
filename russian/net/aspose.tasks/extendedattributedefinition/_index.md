---
title: "Класс ExtendedAttributeDefinition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ExtendedAttributeDefinition. Представляет определение расширенного атрибута, связанного с проектом"
type: docs
weight: 540
url: /ru/net/aspose.tasks/extendedattributedefinition/
---
## ExtendedAttributeDefinition class

Представляет определение расширенного атрибута, связанного с проектом.

```csharp
public class ExtendedAttributeDefinition
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Alias](../../aspose.tasks/extendedattributedefinition/alias/) { get; set; } | Получает или задает псевдоним пользовательского поля. |
| [AppendNewValues](../../aspose.tasks/extendedattributedefinition/appendnewvalues/) { get; set; } | Получает или задает значение, указывающее, добавляются ли новые значения, внесённые в проект, автоматически в список. |
| [AutoRollDown](../../aspose.tasks/extendedattributedefinition/autorolldown/) { get; set; } | Получает или задает значение, указывающее, включено ли автоматическое распространение на назначения. |
| [CalculationType](../../aspose.tasks/extendedattributedefinition/calculationtype/) { get; set; } | Получает или задает тип расчёта значения пользовательского атрибута. |
| [CfType](../../aspose.tasks/extendedattributedefinition/cftype/) { get; } | Получает тип пользовательского поля. |
| [Default](../../aspose.tasks/extendedattributedefinition/default/) { get; set; } | Получает или задает значение по умолчанию в списке. |
| [DefaultGuid](../../aspose.tasks/extendedattributedefinition/defaultguid/) { get; set; } | Получает или задает GUID записи таблицы поиска по умолчанию. |
| [ElementType](../../aspose.tasks/extendedattributedefinition/elementtype/) { get; set; } | Получает или задает, с какой сущностью (задачей, ресурсом или назначением) связан расширенный атрибут. |
| [FieldId](../../aspose.tasks/extendedattributedefinition/fieldid/) { get; set; } | Получает или задает значение, соответствующее идентификатору проекта пользовательского поля. Используйте строковое представление константы из класса [`ExtendedAttributeTask`](../extendedattributetask/) для указания свойства [`FieldId`](./fieldid/). |
| [FieldName](../../aspose.tasks/extendedattributedefinition/fieldname/) { get; } | Получает имя пользовательского поля. |
| [Formula](../../aspose.tasks/extendedattributedefinition/formula/) { get; set; } | Получает или задает формулу, которую Microsoft Project использует для заполнения пользовательского поля задачи. |
| [GraphicalIndicator](../../aspose.tasks/extendedattributedefinition/graphicalindicator/) { get; set; } | Получает или задает информацию о графических индикаторах, связанную с расширенным атрибутом. Применимо к формату MPP. |
| [Guid](../../aspose.tasks/extendedattributedefinition/guid/) { get; set; } | Получает или задает Guid пользовательского поля. |
| [LookupUid](../../aspose.tasks/extendedattributedefinition/lookupuid/) { get; } | Получает Guid таблицы поиска, связанной с пользовательским полем. |
| [MaxMultiValues](../../aspose.tasks/extendedattributedefinition/maxmultivalues/) { get; set; } | Получает или задает максимальное количество значений, которое можно установить в списке выбора. |
| [ParentProject](../../aspose.tasks/extendedattributedefinition/parentproject/) { get; } | Получает родительский проект для экземпляра `ExtendedAttributeDefinition`. |
| [PhoneticsAlias](../../aspose.tasks/extendedattributedefinition/phoneticsalias/) { get; set; } | Получает или задает фонетическое произношение псевдонима пользовательского поля. |
| [RestrictValues](../../aspose.tasks/extendedattributedefinition/restrictvalues/) { get; set; } | Получает или задает значение, указывающее, ограничены ли значения пользовательского поля значениями в [`ValueList`](./valuelist/). |
| [RollupType](../../aspose.tasks/extendedattributedefinition/rolluptype/) { get; set; } | Получает или задает способ расчёта сводных данных. |
| [SecondaryGuid](../../aspose.tasks/extendedattributedefinition/secondaryguid/) { get; set; } | Получает или задает вторичный guid расширенного атрибута. |
| [SecondaryPid](../../aspose.tasks/extendedattributedefinition/secondarypid/) { get; set; } | Получает или задает вторичный PID пользовательского поля. |
| [SummaryRowsCalculationType](../../aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/) { get; set; } | Получает или задает тип расчёта значения пользовательского атрибута для строк итогов. |
| [UserDef](../../aspose.tasks/extendedattributedefinition/userdef/) { get; set; } | Получает или задает значение, указывающее, является ли пользовательское поле определённым пользователем. |
| [ValueList](../../aspose.tasks/extendedattributedefinition/valuelist/) { get; } | Получает List&lt;Value&gt; ValueList. |
| [ValuelistSortOrder](../../aspose.tasks/extendedattributedefinition/valuelistsortorder/) { get; set; } | Получает или задает способ сортировки списков значений. Значения: 0=По убыванию, 1=По возрастанию. |

## Методы

| Имя | Описание |
| --- | --- |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition_1)(ExtendedAttributeResource, string) | Метод фабрики, который создает определение расширенного атрибута с поиском. Он имеет [`CalculationType`](./calculationtype/) равный Lookup и может использоваться только в ресурсах. Требуется указать *fieldId* и *alias* при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateLookupResourceDefinition](../../aspose.tasks/extendedattributedefinition/createlookupresourcedefinition/#createlookupresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Метод фабрики, который создает определение расширенного атрибута с поиском. Он имеет [`CalculationType`](./calculationtype/) равный Lookup и может использоваться только в ресурсах. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition_1)(ExtendedAttributeTask, string) | Метод фабрики, который создает определение расширенного атрибута с поиском. Он имеет [`CalculationType`](./calculationtype/) равный Lookup и может использоваться только в задачах. Требуется указать *fieldId* и *alias* при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateLookupTaskDefinition](../../aspose.tasks/extendedattributedefinition/createlookuptaskdefinition/#createlookuptaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Метод фабрики, который создает определение расширенного атрибута с поиском. Он имеет [`CalculationType`](./calculationtype/) равный Lookup и может использоваться только в задачах. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition_1)(ExtendedAttributeResource, string) | Метод фабрики, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет [`CalculationType`](./calculationtype/) равный None и может использоваться только в ресурсах. Требуется указать *fieldId* и *alias* при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateResourceDefinition](../../aspose.tasks/extendedattributedefinition/createresourcedefinition/#createresourcedefinition)(CustomFieldType, ExtendedAttributeResource, string) | Метод фабрики, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет [`CalculationType`](./calculationtype/) равный None и может использоваться только в ресурсах. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition_1)(ExtendedAttributeTask, string) | Метод фабрики, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет [`CalculationType`](./calculationtype/) равный None и может использоваться только в задачах. Требуется указать *fieldId* и *alias* при вызове этого метода. Тип поля выводится из идентификатора поля. |
| static [CreateTaskDefinition](../../aspose.tasks/extendedattributedefinition/createtaskdefinition/#createtaskdefinition)(CustomFieldType, ExtendedAttributeTask, string) | Метод фабрики, который создает простое определение расширенного атрибута, которое Microsoft Project отображает как "None". Он имеет [`CalculationType`](./calculationtype/) равный None и может использоваться только в задачах. Требуется указать *customFieldType*, *fieldId* и *alias* при вызове этого метода. |
| [AddLookupValue](../../aspose.tasks/extendedattributedefinition/addlookupvalue/)(Value) | Добавляет значение во внутренний список поиска. Это предпочтительный способ работы со [`ValueList`](./valuelist/). |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute)() | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_3)(bool) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением флага. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_4)(DateTime) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением даты. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_5)(decimal) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным числовым значением. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_1)(Duration) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным значением длительности. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_6)(string) | Создает новый расширенный атрибут с идентификатором поля, равным значению идентификатора поля этого объекта, и указанным текстовым значением. |
| [CreateExtendedAttribute](../../aspose.tasks/extendedattributedefinition/createextendedattribute/#createextendedattribute_2)(Value) | Создает новый расширенный атрибут, связанный с указанным элементом [`Value`](../value/). |
| override [Equals](../../aspose.tasks/extendedattributedefinition/equals/)(object) | Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/extendedattributedefinition/gethashcode/)() | Возвращает хеш-код для экземпляра класса `ExtendedAttributeDefinition`. |
| [RemoveLookupValue](../../aspose.tasks/extendedattributedefinition/removelookupvalue/)(Value) | Удаляет значение из внутреннего списка поиска. Это предпочтительный способ работы со [`ValueList`](./valuelist/). |

## Примеры

Показывает, как использовать общие математические функции с расширенными атрибутами.

```csharp
public static void EvaluateChoose()
{
    var project = CreateTestProjectWithCustomField();

    // Установить формулу
    project.ExtendedAttributes[0].Formula = "Choose(3, \"This is a\", \"right\", \"choice\")";

    // Вывести значение расширенного атрибута
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static void EvaluateIsNumeric()
{
    string[] numericFormulas =
        {
            "IsNumeric('AAA')", @"IsNUmeric(1)", "IsNumeric(1<0)", "IsNumeric(\"1.1\")", "IsNumeric(Choose((2 + Sgn(2^-3)), 123, \"one two three\"))"
        };

    var project = CreateTestProjectWithCustomField();

    foreach (var numericFormula in numericFormulas)
    {
        // Установить формулу
        project.ExtendedAttributes[0].Formula = numericFormula;

        // Вывести значение расширенного атрибута
        var task = project.RootTask.Children.GetById(1);
        Console.WriteLine(task.ExtendedAttributes[0].TextValue);
    }
}

public static void EvaluateSwitch()
{
    var project = CreateTestProjectWithCustomField();

    // Установить формулу
    project.ExtendedAttributes[0].Formula = "Switch( 0 < 1, \"0 is lesser than 1\", 0 > 1, \"0 is greater than 1\")";

    // Вывести значение расширенного атрибута
    var task = project.RootTask.Children.GetById(1);
    Console.WriteLine(task.ExtendedAttributes[0].TextValue);
}

public static Project CreateTestProjectWithCustomField()
{
    var project = new Project();
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Text, ExtendedAttributeTask.Text1, "Custom Field");
    project.ExtendedAttributes.Add(definition);

    var task = project.RootTask.Children.Add("Task");

    var attribute = definition.CreateExtendedAttribute();
    task.ExtendedAttributes.Add(attribute);
    return project;
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


