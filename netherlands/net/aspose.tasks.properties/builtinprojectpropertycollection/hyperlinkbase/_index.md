---
title: "BuiltInProjectPropertyCollection.HyperlinkBase"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "BuiltInProjectPropertyCollection eigenschap. Haalt of stelt de hyperlinkbasis van een project in"
type: docs
weight: 50
url: /nl/net/aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/
---
## BuiltInProjectPropertyCollection.HyperlinkBase property

Haalt of stelt de hyperlink‑basis van een project in.

```csharp
public string HyperlinkBase { get; set; }
```

## Voorbeelden

Toont hoe ingebouwde projecteigenschappen te lezen.

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

// itereren over de ingebouwde eigenschapscollectie
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Zie ook

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


