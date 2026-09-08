---
title: "Класс GlobalizationSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.GlobalizationSettings. Представляет глобальные настройки проекта."
type: docs
weight: 720
url: /ru/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Представляет настройки глобализации проекта.

```csharp
public class GlobalizationSettings
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Возвращает строку для булевого литерала 'false', используемого в формуле. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Возвращает литерал \"NA\" (пустое значение), используемый в формуле для поля даты. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Получает строку для булевого литерала 'true', используемого в формуле. |

## Примечания

Рекомендуемый способ — использовать культурно-независимые литералы или форматы по всему проекту. Однако, если проект использует культурно-специфичные литералы, этот класс можно использовать, чтобы помочь движку вычисления формул разбирать эти литералы.

## Примеры

Показывает, как задать языково-специфичные настройки проекта.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Создать расширенный атрибут
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


