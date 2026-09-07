---
title: "CustomProjectPropertyCollection.Remove"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος CustomProjectPropertyCollection. Αφαιρεί μια ιδιότητα με το καθορισμένο όνομα από τη συλλογή."
type: docs
weight: 50
url: /el/net/aspose.tasks.properties/customprojectpropertycollection/remove/
---
## CustomProjectPropertyCollection.Remove method

Αφαιρεί μια ιδιότητα με το καθορισμένο όνομα από τη συλλογή.

```csharp
public bool Remove(string name)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| name | String | Το όνομα της ιδιότητας χωρίς διάκριση πεζών-κεφαλαίων. |

### Τιμή Επιστροφής

Αληθές εάν το στοιχείο βρεθεί και αφαιρεθεί επιτυχώς· διαφορετικά, ψευδές.

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

* class [CustomProjectPropertyCollection](../)
* namespace [Aspose.Tasks.Properties](../../customprojectpropertycollection/)
* assembly [Aspose.Tasks](../../../)


