---
title: "BuiltInProjectProperty.Value"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "BuiltInProjectProperty property. Haalt de waarde op of stelt deze in van de eigenschap"
type: docs
weight: 10
url: /nl/net/aspose.tasks.properties/builtinprojectproperty/value/
---
## BuiltInProjectProperty.Value property

Haalt de waarde op of stelt deze in van de eigenschap.

```csharp
public string Value { get; set; }
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

* class [BuiltInProjectProperty](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectproperty/)
* assembly [Aspose.Tasks](../../../)


