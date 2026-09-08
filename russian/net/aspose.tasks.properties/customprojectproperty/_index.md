---
title: "Класс CustomProjectProperty"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Properties.CustomProjectProperty. Представляет пользовательское свойство"
type: docs
weight: 1540
url: /ru/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

Представляет пользовательское свойство.

```csharp
public sealed class CustomProjectProperty : Property
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Получает имя свойства. |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | Получает тип свойства. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Получает или задает значение свойства. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Возвращает значение свойства в виде строки. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


