---
title: "BuiltInProjectPropertyCollection.Author"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "BuiltInProjectPropertyCollection property. Λαμβάνει ή ορίζει τον συγγραφέα ενός έργου"
type: docs
weight: 10
url: /el/net/aspose.tasks.properties/builtinprojectpropertycollection/author/
---
## BuiltInProjectPropertyCollection.Author property

Λαμβάνει ή ορίζει τον συγγραφέα ενός έργου.

```csharp
public string Author { get; set; }
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


