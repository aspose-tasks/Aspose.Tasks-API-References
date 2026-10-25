---
title: "Project.BuiltInProps"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство Project. Получает коллекцию встроенных свойств проекта"
type: docs
weight: 100
url: /ru/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Получает встроенную коллекцию свойств проекта.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
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

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


