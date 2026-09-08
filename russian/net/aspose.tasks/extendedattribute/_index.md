---
title: "Класс ExtendedAttribute"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ExtendedAttribute. Представляет расширенные атрибуты"
type: docs
weight: 520
url: /ru/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Представляет расширенные атрибуты.

```csharp
public class ExtendedAttribute
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Получает определение атрибута. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Получает или задает значение для атрибутов с типами даты (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Получает или задает значение для атрибутов типа 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Получает идентификатор поля. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Получает или задает значение, указывающее, установлен ли флаг для атрибута типа 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Определяет, привела ли вычисление значения расширенного атрибута к ошибке. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Получает или задает значение для атрибутов с числовыми типами (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Получает или задает значение для атрибутов типа 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Получает GUID значения справочника. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Получает значение, указывающее, является ли значение данного экземпляра `ExtendedAttribute` только для чтения. Возвращает true, если формула или агрегирование определены в [`ExtendedAttributeDefinition`](../extendedattributedefinition/) для этого объекта. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Возвращает краткое строковое представление расширенного атрибута. |

## Примечания

В настоящее время поддерживаются все типы расширенных атрибутов, читаемые из MSP Xml 2003/2007 и mpp 2003. Для MSP mpp 2007 поддерживается чтение всех расширенных атрибутов, кроме длительностей и флагов.

## Примеры

Показывает, как добавить пользовательское поле, значение которого рассчитывается с помощью формулы, указанной пользователем.

```csharp
var project = new Project();

// создать новое определение расширенного атрибута задачи
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Добавьте формулу к атрибуту.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Создать расширенный атрибут
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Мы задаем Формулу для расширенного атрибута, поэтому он только для чтения (значение рассчитывается с помощью формулы).
// Вывод: "Значение только для чтения"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Вы можете попытаться установить значение только для чтения поля, но это не даст эффекта.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


