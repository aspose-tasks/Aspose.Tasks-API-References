---
title: "Класс Value"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Value. Представляет значение в списке значений"
type: docs
weight: 2800
url: /ru/net/aspose.tasks/value/
---
## Value class

Представляет значение в списке значений.

```csharp
public class Value
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Value](value/)() | Инициализирует новый экземпляр класса `Value`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | Возвращает или задает фактическое значение, если оно может быть представлено как DateTime. Значение по умолчанию — MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | Возвращает или задает описание значения. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | Возвращает или задает фактическое значение, используемое для представления длительности. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | Возвращает или задает уникальный идентификатор значения в рамках проекта. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | Возвращает или задает фактическое значение, используемое для представления числового или стоимостного значения. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | Возвращает или задает фонетическую информацию о названии пользовательского поля. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | Возвращает или задает фактическое значение, используемое для представления текстовой строки. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | Возвращает или задает фактическое значение во внутреннем представлении. Предпочтительно использовать строго типизированные свойства, перечисленные ниже. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | Возвращает GUID, который идентифицирует это значение среди остальных во всём проекте. |

## Примеры

Показывает, как работать с lookup‑значениями.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// Создайте определение расширенного атрибута типа Text
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// Добавьте lookup‑значения для определения расширенного атрибута
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Создайте определение расширенного атрибута типа Duration
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// Добавьте lookup‑значения для определения расширенного атрибута
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Создайте определение расширенного атрибута типа Date
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// Создайте определение расширенного атрибута типа Number
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


