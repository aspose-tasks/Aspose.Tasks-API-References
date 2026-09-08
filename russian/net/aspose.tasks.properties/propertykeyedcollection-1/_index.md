---
title: "Класс PropertyKeyedCollectionT"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Properties.PropertyKeyedCollection1T. Базовый класс коллекции свойств"
type: docs
weight: 1600
url: /ru/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Базовый класс коллекции свойств.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Параметр | Описание |
| --- | --- |
| T | Тип свойства. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Получает количество свойств в коллекции. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Получает свойство, связанное с указанным ключом. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Получает коллекцию всех имен свойств. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Создает новое пользовательское свойство. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Определяет, содержит ли [`PropertyCollection`](../propertycollection-1/) свойство с указанным именем. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


