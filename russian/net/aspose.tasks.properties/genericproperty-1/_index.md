---
title: "Структура GenericPropertyTKey"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Структура Aspose.Tasks.Properties.GenericProperty1TKey. Представляет контейнерное свойство"
type: docs
weight: 1570
url: /ru/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Представляет свойство контейнера.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Параметр | Описание |
| --- | --- |
| TKey | Тип значения свойства. |

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Инициализирует новый экземпляр структуры `GenericProperty`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Получает имя свойства. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Получает значение свойства. |

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


