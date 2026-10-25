---
title: "Κλάση BuiltInProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.BuiltInProjectPropertyCollection κλάση. Αντιπροσωπεύει μια συλλογή ενσωματωμένων ιδιοτήτων έργου"
type: docs
weight: 1530
url: /el/net/aspose.tasks.properties/builtinprojectpropertycollection/
---
## BuiltInProjectPropertyCollection class

Αναπαριστά μια συλλογή ενσωματωμένων ιδιοτήτων έργου.

```csharp
public sealed class BuiltInProjectPropertyCollection : 
    PropertyKeyedCollection<BuiltInProjectProperty>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Author](../../aspose.tasks.properties/builtinprojectpropertycollection/author/) { get; set; } | Λαμβάνει ή ορίζει τον συγγραφέα ενός έργου. |
| [Category](../../aspose.tasks.properties/builtinprojectpropertycollection/category/) { get; set; } | Λαμβάνει ή ορίζει την κατηγορία ενός έργου. |
| [Comments](../../aspose.tasks.properties/builtinprojectpropertycollection/comments/) { get; set; } | Λαμβάνει ή ορίζει τα σχόλια ενός έργου. |
| [Company](../../aspose.tasks.properties/builtinprojectpropertycollection/company/) { get; set; } | Λαμβάνει ή ορίζει την εταιρεία ενός έργου. |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| [HyperlinkBase](../../aspose.tasks.properties/builtinprojectpropertycollection/hyperlinkbase/) { get; set; } | Λαμβάνει ή ορίζει τη βάση υπερσυνδέσμου ενός έργου. |
| override [IsReadOnly](../../aspose.tasks.properties/builtinprojectpropertycollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Keywords](../../aspose.tasks.properties/builtinprojectpropertycollection/keywords/) { get; set; } | Λαμβάνει ή ορίζει τις λέξεις-κλειδιά ενός έργου. |
| [Manager](../../aspose.tasks.properties/builtinprojectpropertycollection/manager/) { get; set; } | Λαμβάνει ή ορίζει τον διαχειριστή ενός έργου. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |
| [Subject](../../aspose.tasks.properties/builtinprojectpropertycollection/subject/) { get; set; } | Λαμβάνει ή ορίζει το θέμα ενός έργου. |
| [Title](../../aspose.tasks.properties/builtinprojectpropertycollection/title/) { get; set; } | Λαμβάνει ή ορίζει τον τίτλο ενός έργου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(BuiltInProjectProperty) |  |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις ενσωματωμένες ιδιότητες του έργου.

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

// επανάληψη πάνω στη συλλογή ενσωματωμένων ιδιοτήτων
foreach (Property property in project.BuiltInProps)
{
    Console.WriteLine("Name: " + property.Name);
    Console.WriteLine("Value: " + property.Value);
    Console.WriteLine("Prop As String: " + property.ToString());
    Console.WriteLine();
}
```

### Δείτε επίσης

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [BuiltInProjectProperty](../builtinprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


