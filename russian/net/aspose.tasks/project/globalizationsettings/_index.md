---
title: "Project.GlobalizationSettings"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает или задает глобализационные языко-специфические настройки проекта"
type: docs
weight: 460
url: /ru/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Получает или задает глобализационные (языко-специфичные) настройки проекта.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Примечания

Рекомендуемый способ — использовать независимые от культуры литералы или форматы во всём проекте. Однако, если проект использует литералы, зависящие от культуры, этот класс можно использовать, чтобы помочь движку расчётов разобрать эти литералы.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


