---
title: "Класс Property"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Properties.Property. Представляет базовый класс свойства"
type: docs
weight: 1580
url: /ru/net/aspose.tasks.properties/property/
---
## Property class

Представляет базовый класс свойства.

```csharp
public abstract class Property
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Получает имя свойства. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Получает или задает значение свойства. |

## Методы

| Имя | Описание |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Возвращает значение свойства в виде строки. |

## Примеры

Показывает, как читать встроенные свойства проекта.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Author: " + project.BuiltInProps.Author);
Console.WriteLine("Category: " + project.BuiltInProps.Category);
Console.WriteLine("Comments: " + project.BuiltInProps.Comments);
Console.WriteLine("Company: " + project.BuiltInProps.Company);
Console.WriteLine("HyperlinkBase: " + project.BuiltInProps.HyperlinkBase);
Console.WriteLine("IsReadOnly: " + project.BuiltInProps.IsReadOnly);
Console.WriteLine("Keywords: " + project.BuiltInProps.Keywords);
Console.WriteLine("Manager: " + project.BuiltInProps.Manager);
Console.WriteLine("Subject: " + project.BuiltInProps.Subject);
Console.WriteLine("Title: " + project.BuiltInProps.Title);
Console.WriteLine();

// перебрать коллекцию встроенных свойств
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### См. также

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


