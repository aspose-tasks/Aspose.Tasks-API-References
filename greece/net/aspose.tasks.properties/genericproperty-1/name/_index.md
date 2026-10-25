---
title: "GenericProperty1.Name"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "GenericProperty property. Ανακτά ένα όνομα της ιδιότητας"
type: docs
weight: 20
url: /el/net/aspose.tasks.properties/genericproperty-1/name/
---
## GenericProperty&lt;TKey&gt;.Name property

Λαμβάνει ένα όνομα της ιδιότητας.

```csharp
public string Name { get; }
```

## Παραδείγματα

Δείχνει πώς να εργαστείτε με προσαρμοσμένες συλλογές ιδιοτήτων έργου.

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// Ας προσθέσουμε νέες προσαρμοσμένες ιδιότητες
// Η συλλογή υποστηρίζει τύπους Boolean, DateTime, Double, String
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// Οι προσαρμοσμένες ιδιότητες είναι διαθέσιμες μέσω της τυποποιημένης συλλογής
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// Λάβετε μια τιμή προσαρμοσμένης ιδιότητας
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// Επανάληψη πάνω στα ονόματα των προσαρμοσμένων ιδιοτήτων
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// Μπορείτε να διαγράψετε μια τιμή με κλειδί συμβολοσειράς
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// ή μπορεί κανείς να καθαρίσει τη συλλογή εντελώς
project.CustomProps.Clear();
```

### Δείτε επίσης

* struct [GenericProperty&lt;TKey&gt;](../)
* namespace [Aspose.Tasks.Properties](../../genericproperty-1/)
* assembly [Aspose.Tasks](../../../)


