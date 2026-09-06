---
title: "Project.CustomProps"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété du projet. Obtient la collection des propriétés personnalisées du projet"
type: docs
weight: 260
url: /fr/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

Obtient la collection des propriétés personnalisées du projet.

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## Exemples

Montre comment lire les méta-propriétés du projet (API obsolète).

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// les propriétés personnalisées sont disponibles via la collection typée
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// les propriétés intégrées sont disponibles directement
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// ou comme un élément de la collection de propriétés intégrées
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### Voir aussi

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


