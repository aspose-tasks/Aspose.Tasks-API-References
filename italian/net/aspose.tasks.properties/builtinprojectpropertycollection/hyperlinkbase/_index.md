---
title: "BuiltInProjectPropertyCollection.HyperlinkBase"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "BuiltInProjectPropertyCollection property. Ottiene o imposta la base dei collegamenti ipertestuali di un progetto"
type: docs
weight: 50
url: /it/net/aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/
---
## BuiltInProjectPropertyCollection.HyperlinkBase property

Ottiene o imposta la base dei collegamenti ipertestuali di un progetto.

```csharp
public string HyperlinkBase { get; set; }
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


