---
title: "BuiltInProjectProperty.Value"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство BuiltInProjectProperty. Получает или задает значение свойства"
type: docs
weight: 10
url: /ru/net/aspose.tasks.properties/builtinprojectproperty/value/
---
## BuiltInProjectProperty.Value property

Получает или задает значение свойства.

```csharp
public string Value { get; set; }
```

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

* class [BuiltInProjectProperty](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectproperty/)
* assembly [Aspose.Tasks](../../../)


