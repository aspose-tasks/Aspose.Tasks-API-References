---
title: "Класс BuiltInProjectProperty"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Properties.BuiltInProjectProperty. Представляет встроенное свойство."
type: docs
weight: 1520
url: /ru/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Представляет встроенное свойство.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Получает имя свойства. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Получает или задает значение свойства. (2 свойства) |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


