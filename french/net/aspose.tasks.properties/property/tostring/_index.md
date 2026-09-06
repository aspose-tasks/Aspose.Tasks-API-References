---
title: "Property.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Property. Retourne la valeur de la propriété sous forme de chaîne"
type: docs
weight: 30
url: /fr/net/aspose.tasks.properties/property/tostring/
---
## Property.ToString method

Renvoie la valeur de la propriété sous forme de chaîne.

```csharp
public override string ToString()
```

### Valeur de retour

Valeur de chaîne.

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

* class [Property](../)
* namespace [Aspose.Tasks.Properties](../../property/)
* assembly [Aspose.Tasks](../../../)


