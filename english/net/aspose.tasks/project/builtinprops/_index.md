---
title: Project.BuiltInProps
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets projects builtin properties collection
type: docs
weight: 100
url: /net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Gets project's built-in properties collection.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## Examples

Shows how to read project meta properties (obsolete API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// custom properties are available through the typed collection
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// built-in properties are available directly
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// or as an item of built-in property collection
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### See Also

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


