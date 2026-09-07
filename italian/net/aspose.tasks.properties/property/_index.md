---
title: "Classe Property"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Properties.Property. Rappresenta una classe base di una proprietà"
type: docs
weight: 1580
url: /it/net/aspose.tasks.properties/property/
---
## Property class

Rappresenta una classe base di una proprietà.

```csharp
public abstract class Property
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Ottiene il nome della proprietà. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Ottiene o imposta un valore della proprietà. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Restituisce il valore della proprietà come stringa. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


