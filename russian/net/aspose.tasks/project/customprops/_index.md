---
title: "Project.CustomProps"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает коллекцию пользовательских свойств проекта"
type: docs
weight: 260
url: /ru/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Получает коллекцию пользовательских свойств проекта.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## Примеры

Показывает, как читать метасвойства проекта (устаревший API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// пользовательские свойства доступны через типизированную коллекцию
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Встроенные свойства доступны напрямую
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// или как элемент коллекции встроенных свойств
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### См. также

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


