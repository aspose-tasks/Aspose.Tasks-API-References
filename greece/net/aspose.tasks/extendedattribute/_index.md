---
title: "Κλάση ExtendedAttribute"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ExtendedAttribute class. Αντιπροσωπεύει επεκτατικά χαρακτηριστικά"
type: docs
weight: 520
url: /el/net/aspose.tasks/extendedattribute/
---
## ExtendedAttribute class

Αντιπροσωπεύει επεκταμένα χαρακτηριστικά.

```csharp
public class ExtendedAttribute
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [AttributeDefinition](../../aspose.tasks/extendedattribute/attributedefinition/) { get; } | Λαμβάνει τον ορισμό του χαρακτηριστικού. |
| [DateValue](../../aspose.tasks/extendedattribute/datevalue/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά με τύπους ημερομηνίας (Date, Start, Finish). |
| [DurationValue](../../aspose.tasks/extendedattribute/durationvalue/) { get; set; } | Λαμβάνει ή ορίζει τιμή για χαρακτηριστικά τύπου 'Duration'. |
| [FieldId](../../aspose.tasks/extendedattribute/fieldid/) { get; } | Λαμβάνει το αναγνωριστικό (id) ενός πεδίου. |
| [FlagValue](../../aspose.tasks/extendedattribute/flagvalue/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν έχει οριστεί σημαία για χαρακτηριστικό τύπου 'Flag'. |
| [IsErrorValue](../../aspose.tasks/extendedattribute/iserrorvalue/) { get; } | Λαμβάνει εάν ο υπολογισμός της τιμής του επεκτατικού χαρακτηριστικού οδήγησε σε σφάλμα. |
| [NumericValue](../../aspose.tasks/extendedattribute/numericvalue/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά με αριθμητικούς τύπους (Cost, Number). |
| [TextValue](../../aspose.tasks/extendedattribute/textvalue/) { get; set; } | Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά τύπου 'Text'. |
| [ValueGuid](../../aspose.tasks/extendedattribute/valueguid/) { get; } | Λαμβάνει το guid μιας τιμής αναζήτησης. |
| [ValueReadOnly](../../aspose.tasks/extendedattribute/valuereadonly/) { get; } | Λαμβάνει μια τιμή που υποδεικνύει εάν μια τιμή αυτής της `ExtendedAttribute` παρουσίας είναι μόνο για ανάγνωση. Επιστρέφει true εάν ορίζεται formula ή rollup στο [`ExtendedAttributeDefinition`](../extendedattributedefinition/) για αυτό το αντικείμενο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ToString](../../aspose.tasks/extendedattribute/tostring/)() | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός επεκτατικού χαρακτηριστικού. |

## Παρατηρήσεις

Προς το παρόν υποστηρίζονται όλοι οι τύποι επεκτατικών χαρακτηριστικών που διαβάζονται από MSP Xml 2003/2007 και mpp 2003. Για MSP mpp 2007 υποστηρίζεται η ανάγνωση όλων των επεκτατικών χαρακτηριστικών εκτός από διάρκειες και σημαίες.

## Παραδείγματα

Δείχνει πώς να προσθέσετε προσαρμοσμένο πεδίο του οποίου η τιμή υπολογίζεται χρησιμοποιώντας τύπο που καθορίζεται από τον χρήστη.

```csharp
var project = new Project();

// δημιουργήστε νέο ορισμό επεκτατικού χαρακτηριστικού εργασίας
var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, "Cost ratio");

// Προσθέστε τύπο στο χαρακτηριστικό.
attribute.Formula = "[Cost] / [Actual Cost]";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Δημιουργία εκτεταμένου χαρακτηριστικού
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

// Ορίζουμε το Formula για το επεκτατικό χαρακτηριστικό, ώστε να είναι μόνο για ανάγνωση (η τιμή υπολογίζεται χρησιμοποιώντας τύπο).
// Η έξοδος είναι "Value is read only"
Console.WriteLine(extendedAttribute.ValueReadOnly ? "Value is read only" : "Value is not read only");

// Μπορείτε να προσπαθήσετε να ορίσετε τιμή σε πεδίο μόνο για ανάγνωση, αλλά δεν θα έχει αποτέλεσμα.
extendedAttribute.NumericValue = -1000000M;

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost),
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());

task.Set(Tsk.Cost, 100m);
task.Set(Tsk.ActualCost, 120m);

Console.WriteLine("Cost is {0}, Actual Cost is {1}, Custom attribute's value is {2}",
    task.Get(Tsk.Cost), 
    task.Get(Tsk.ActualCost),
    extendedAttribute.IsErrorValue ? "#Error" : extendedAttribute.NumericValue.ToString());
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


