---
title: "Δομή GenericPropertyTKey"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.GenericProperty1TKey δομή. Αντιπροσωπεύει μια ιδιότητα δοχείου"
type: docs
weight: 1570
url: /el/net/aspose.tasks.properties/genericproperty-1/
---
## GenericProperty&lt;TKey&gt; structure

Αντιπροσωπεύει μια ιδιότητα δοχείου.

```csharp
public struct GenericProperty<TKey>
    where TKey : struct
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| TKey | Ο τύπος της τιμής ιδιότητας. |

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GenericProperty](genericproperty/)(string) | Αρχικοποιεί μια νέα παρουσία της δομής `GenericProperty`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Name](../../aspose.tasks.properties/genericproperty-1/name/) { get; } | Λαμβάνει ένα όνομα της ιδιότητας. |
| [Value](../../aspose.tasks.properties/genericproperty-1/value/) { get; } | Λαμβάνει μια τιμή της ιδιότητας. |

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

* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


