---
title: "Класс CustomProjectPropertyCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Properties.CustomProjectPropertyCollection. Представляет коллекцию пользовательских свойств проекта"
type: docs
weight: 1550
url: /ru/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

Представляет коллекцию пользовательских свойств проекта.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | Инициализирует новый экземпляр класса `CustomProjectPropertyCollection`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения; в противном случае — false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | Создает новое пользовательское свойство. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | Создает новое пользовательское свойство. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | Создает новое пользовательское свойство. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | Создает новое пользовательское свойство. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | Очищает PropertyCollection. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | Удаляет свойство с указанным именем из коллекции. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


