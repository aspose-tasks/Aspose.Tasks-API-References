---
title: "BuiltInProjectPropertyCollection.Comments"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "BuiltInProjectPropertyCollection property. Ανακτά ή ορίζει τα σχόλια ενός έργου"
type: docs
weight: 30
url: /el/net/aspose.tasks.properties/builtinprojectpropertycollection/comments/
---
## BuiltInProjectPropertyCollection.Comments property

Λαμβάνει ή ορίζει τα σχόλια ενός έργου.

```csharp
public string Comments { get; set; }
```

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

* class [BuiltInProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../builtinprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


