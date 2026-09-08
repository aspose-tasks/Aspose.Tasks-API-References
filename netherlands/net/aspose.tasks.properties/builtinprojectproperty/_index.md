---
title: "Klasse BuiltInProjectProperty"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Properties.BuiltInProjectProperty klasse. Vertegenwoordigt een ingebouwde eigenschap"
type: docs
weight: 1520
url: /nl/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Stelt een ingebouwde eigenschap voor.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Haalt de naam van de eigenschap op. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Haalt of stelt de waarde van de eigenschap in. (2 eigenschappen) |

## Methoden

| Naam | Beschrijving |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Retourneert de eigenschapswaarde als string. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


