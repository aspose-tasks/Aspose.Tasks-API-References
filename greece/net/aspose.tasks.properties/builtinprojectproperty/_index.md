---
title: "Κλάση BuiltInProjectProperty"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.BuiltInProjectProperty κλάση. Αντιπροσωπεύει μια ενσωματωμένη ιδιότητα"
type: docs
weight: 1520
url: /el/net/aspose.tasks.properties/builtinprojectproperty/
---
## BuiltInProjectProperty class

Αναπαριστά μια ενσωματωμένη ιδιότητα.

```csharp
public sealed class BuiltInProjectProperty : Property
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Λαμβάνει ένα όνομα της ιδιότητας. |
| [Value](../../aspose.tasks.properties/builtinprojectproperty/value/) { get; set; } | Λαμβάνει ή ορίζει την τιμή της ιδιότητας. (2 ιδιότητες) |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | Επιστρέφει την τιμή της ιδιότητας ως συμβολοσειρά. |

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

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


