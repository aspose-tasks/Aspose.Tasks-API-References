---
title: "Classe Property"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Properties.Property. Représente une classe de base d'une propriété"
type: docs
weight: 1580
url: /fr/net/aspose.tasks.properties/property/
---
## Property class

Représente une classe de base d'une propriété.

```csharp
public abstract class Property
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Obtient le nom de la propriété. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Obtient ou définit une valeur de la propriété. |

## Méthodes

| Nom | Description |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Renvoie la valeur de la propriété sous forme de chaîne. |

## Exemples

Montre comment lire les propriétés intégrées du projet.

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

// itérer sur la collection de propriétés intégrées
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Voir aussi

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


