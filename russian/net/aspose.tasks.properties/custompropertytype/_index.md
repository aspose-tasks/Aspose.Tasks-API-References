---
title: "Перечисление CustomPropertyType"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Перечисление Aspose.Tasks.Properties.CustomPropertyType. Представляет перечисление типов пользовательских свойств"
type: docs
weight: 1560
url: /ru/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

Представляет перечисление типов пользовательских свойств.

```csharp
public enum CustomPropertyType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| None | `0` | Свойство не имеет типа. |
| String | `1` | Свойство имеет строковое значение. |
| DateTime | `2` | Свойство имеет значение даты и времени. |
| Number | `3` | Свойство имеет целочисленное значение. |
| Boolean | `4` | Свойство имеет логическое значение. |

## Примеры

Показывает, как работать с пользовательскими коллекциями свойств проекта.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// добавим новые пользовательские свойства
// коллекция поддерживает типы Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// пользовательские свойства доступны через типизированную коллекцию
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// получить значение пользовательского свойства
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// перебрать имена пользовательских свойств
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// можно удалить значение по строковому ключу
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// или можно полностью очистить коллекцию
project.CustomProps.Clear();
```

### См. также

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


