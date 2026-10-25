---
title: "Κλάση Property"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.Property κλάση. Αντιπροσωπεύει μια βασική κλάση μιας ιδιότητας"
type: docs
weight: 1580
url: /el/net/aspose.tasks.properties/property/
---
## Property class

Αναπαριστά μια βασική κλάση μιας ιδιότητας.

```csharp
public abstract class Property
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | Λαμβάνει ένα όνομα της ιδιότητας. |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή της ιδιότητας. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


