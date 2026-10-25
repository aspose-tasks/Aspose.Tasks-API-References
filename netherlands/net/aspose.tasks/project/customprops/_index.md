---
title: "Project.CustomProps"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project eigenschap. Haalt de collectie van aangepaste projecteigenschappen op."
type: docs
weight: 260
url: /nl/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Haalt de aangepaste eigenschapencollectie van het project op.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
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

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


