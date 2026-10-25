---
title: "Κλάση PropertyKeyedCollectionT"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.Properties.PropertyKeyedCollection1T κλάση. Μια βασική κλάση συλλογής ιδιοτήτων"
type: docs
weight: 1600
url: /el/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

Βασική κlass συλλογής ιδιοτήτων.

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| T | Ο τύπος της ιδιότητας. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | Λαμβάνει τον αριθμό των ιδιοτήτων στη συλλογή. |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν αυτή η συλλογή είναι μόνο για ανάγνωση· διαφορετικά, false. |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | Λαμβάνει την Property που συσχετίζεται με το καθορισμένο κλειδί. |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | Λαμβάνει τη συλλογή όλων των ονομάτων ιδιοτήτων. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | Δημιουργεί μια νέα προσαρμοσμένη ιδιότητα. |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | Καθορίζει εάν το [`PropertyCollection`](../propertycollection-1/) περιέχει μια ιδιότητα με το καθορισμένο όνομα. |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


