---
title: "ExtendedAttribute.DurationValue"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ExtendedAttribute. Получает или задает значение для атрибутов типа Duration"
type: docs
weight: 30
url: /ru/net/aspose.tasks/extendedattribute/durationvalue/
---
## ExtendedAttribute.DurationValue property

Получает или задает значение для атрибутов типа 'Duration'.

```csharp
public Duration DurationValue { get; set; }
```

### Исключения

| исключение | условие |
| --- | --- |
| InvalidOperationException | Выбрасывается, если свойство [`AttributeDefinition`](../attributedefinition/) не инициализировано или тип пользовательского поля свойства [`AttributeDefinition`](../attributedefinition/) не является экземпляром [`Duration`](../../duration/). |

## Примеры

Показывает, как добавить расширенные атрибуты, использующие формулы даты/времени MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Установите формулу ProjDateDiff и выведите значение расширенного атрибута
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// Установите формулу ProjDateSub и выведите значение расширенного атрибута
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Мы можем установить формулу ProjDurConv для атрибута со значением длительности, а также для атрибута со значением текста.
// Установите формулу ProjDurConv для расширенного атрибута со значением длительности и выведите его значение.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Установите формулу ProjDurConv для расширенного атрибута со значением текста и выведите его значение.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Установите формулу Second и выведите значение расширенного атрибута.
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Установите формулу Weekday и выведите значение расширенного атрибута.
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### См. также

* struct [Duration](../../duration/)
* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


