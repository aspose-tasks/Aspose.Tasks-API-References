---
title: "BuiltInProjectPropertyCollection.HyperlinkBase"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété BuiltInProjectPropertyCollection. Obtient ou définit la base de lien hypertexte d'un projet"
type: docs
weight: 50
url: /fr/net/aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/
---
## BuiltInProjectPropertyCollection.HyperlinkBase property

Obtient ou définit la base du lien hypertexte d'un projet.

```csharp
public string HyperlinkBase { get; set; }
```

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

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


