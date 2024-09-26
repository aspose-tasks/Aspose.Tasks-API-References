---
title: Project.CustomProps
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets projects custom properties collection
type: docs
weight: 260
url: /net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Gets project's custom properties collection.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
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

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


