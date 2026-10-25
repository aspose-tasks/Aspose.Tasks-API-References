---
title: "BuiltInProjectPropertyCollection.IsReadOnly"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "BuiltInProjectPropertyCollection property. Restituisce un valore che indica se questa collezione è di sola lettura, altrimenti false"
type: docs
weight: 60
url: /it/net/aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/
---
## BuiltInProjectPropertyCollection.IsReadOnly property

Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false.

```csharp
public override bool IsReadOnly { get; }
```

## Esempi

Mostra come leggere le proprietà integrate del progetto.

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

// itera sulla collezione di proprietà integrate
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Vedi anche

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


