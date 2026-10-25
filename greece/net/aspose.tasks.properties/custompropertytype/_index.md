---
title: "Απαρίθμηση CustomPropertyType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.CustomPropertyType απαρίθμηση. Αντιπροσωπεύει μια απαρίθμηση τύπου προσαρμοσμένης ιδιότητας"
type: docs
weight: 1560
url: /el/net/aspose.tasks.properties/custompropertytype/
---
## CustomPropertyType enumeration

Αντιπροσωπεύει μια απαρίθμηση τύπου προσαρμοσμένης ιδιότητας.

```csharp
public enum CustomPropertyType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Η ιδιότητα δεν έχει τύπο. |
| String | `1` | Η ιδιότητα είναι τιμή συμβολοσειράς. |
| DateTime | `2` | Η ιδιότητα είναι τιμή ημερομηνίας και ώρας. |
| Number | `3` | Η ιδιότητα είναι ακέραιος αριθμός. |
| Boolean | `4` | Η ιδιότητα είναι λογική τιμή. |

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


