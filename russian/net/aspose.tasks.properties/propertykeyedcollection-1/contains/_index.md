---
title: "PropertyKeyedCollection1.Contains"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод PropertyKeyedCollection. Определяет, содержит ли PropertyCollection свойство с указанным именем"
type: docs
weight: 60
url: /ru/net/aspose.tasks.properties/propertykeyedcollection-1/contains/
---
## PropertyKeyedCollection&lt;T&gt;.Contains method

Определяет, содержит ли [`PropertyCollection`](../../propertycollection-1/) свойство с указанным именем.

```csharp
public bool Contains(string name)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | Строка | Имя свойства |

### Возвращаемое значение

true, если [`PropertyCollection`](../../propertycollection-1/) содержит свойство с указанным именем; иначе false.

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


