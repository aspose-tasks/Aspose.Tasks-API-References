---
title: "PropertyKeyedCollection1.Item"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство PropertyKeyedCollection. Получает свойство, связанное с указанным ключом"
type: docs
weight: 30
url: /ru/net/aspose.tasks.properties/propertykeyedcollection-1/item/
---
## PropertyKeyedCollection&lt;T&gt; indexer

Получает свойство, связанное с указанным ключом.

```csharp
public T this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя свойства, которое нужно получить. |

### Возвращаемое значение

Свойство, связанное с указанным именем.

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

* class [PropertyKeyedCollection&lt;T&gt;](../)
* namespace [Aspose.Tasks.Properties](../../propertykeyedcollection-1/)
* assembly [Aspose.Tasks](../../../)


