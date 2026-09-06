---
title: "BuiltInProjectProperty.Value"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété BuiltInProjectProperty. Obtient ou définit la valeur de la propriété"
type: docs
weight: 10
url: /fr/net/aspose.tasks.properties/builtinprojectproperty/value/
---
## BuiltInProjectProperty.Value property

Obtient ou définit la valeur de la propriété.

```csharp
public string Value { get; set; }
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

* class [BuiltInProjectProperty](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectproperty/)
* assembly [Aspose.Tasks](../../../)


