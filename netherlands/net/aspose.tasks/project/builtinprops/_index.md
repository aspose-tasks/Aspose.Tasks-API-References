---
title: "Project.BuiltInProps"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt de ingebouwde eigenschappenverzameling van het project op"
type: docs
weight: 100
url: /nl/net/aspose.tasks/project/builtinprops/
---
## Project.BuiltInProps property

Haalt de ingebouwde eigenschapencollectie van het project op.

```csharp
public BuiltInProjectPropertyCollection BuiltInProps { get; }
```

## Voorbeelden

Toont hoe projectmeta-eigenschappen gelezen kunnen worden (verouderde API).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// Aangepaste eigenschappen zijn beschikbaar via de getypeerde collectie
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// Ingebouwde eigenschappen zijn direct beschikbaar
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// of als een item van de ingebouwde eigenschapencollectie
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Zie ook

* class [BuiltInProjectPropertyCollection](../../../aspose.tasks.properties/builtinprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


