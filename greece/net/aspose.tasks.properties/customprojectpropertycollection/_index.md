---
title: "Κλάση CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.CustomProjectPropertyCollection κλάση. Αντιπροσωπεύει μια συλλογή προσαρμοσμένων ιδιοτήτων έργου"
type: docs
weight: 1550
url: /el/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

Αναπαριστά μια συλλογή προσαρμοσμένων ιδιοτήτων έργου.

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `CustomProjectPropertyCollection`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | Καθαρίζει το PropertyCollection. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | Αφαιρεί μια ιδιότητα με το καθορισμένο όνομα από τη συλλογή. |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


