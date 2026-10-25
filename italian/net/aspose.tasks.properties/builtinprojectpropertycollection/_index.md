---
title: "Classe BuiltInProjectPropertyCollection"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Properties.BuiltInProjectPropertyCollection. Rappresenta una collezione di proprietà integrate del progetto"
type: docs
weight: 1530
url: /it/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

Rappresenta una raccolta di proprietà di progetto integrate.

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | Ottiene o imposta l'autore di un progetto. |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | Ottiene o imposta la categoria di un progetto. |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | Ottiene o imposta i commenti di un progetto. |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | Ottiene o imposta l'azienda di un progetto. |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | Ottiene o imposta la base dei collegamenti ipertestuali di un progetto. |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | Restituisce un valore che indica se questa collezione è di sola lettura; altrimenti, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | Ottiene o imposta le parole chiave di un progetto. |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | Ottiene o imposta il responsabile di un progetto. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | Ottiene o imposta l'oggetto di un progetto. |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | Ottiene o imposta il titolo di un progetto. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


