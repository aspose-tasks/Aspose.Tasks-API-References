---
title: "ExtendedAttribute.TextValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttribute. Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά με τύπο Text"
type: docs
weight: 80
url: /el/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά τύπου 'Text'.

```csharp
public string TextValue { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται εάν η ιδιότητα [`AttributeDefinition`](../attributedefinition/) δεν έχει αρχικοποιηθεί ή το τρέχον χαρακτηριστικό δεν είναι χαρακτηριστικό κειμένου. |

## Παραδείγματα

Δείχνει πώς να προσθέσετε εκτεταμένα χαρακτηριστικά που χρησιμοποιούν τύπους ημερομηνίας/ώρας του MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// Ορίστε τον τύπο ProjDateDiff και εκτυπώστε την τιμή του εκτεταμένου χαρακτηριστικού.
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// Ορίστε τον τύπο ProjDateSub και εκτυπώστε την τιμή του εκτεταμένου χαρακτηριστικού.
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// Μπορούμε να ορίσουμε τον τύπο ProjDurConv σε χαρακτηριστικό με τιμή διάρκειας καθώς και σε χαρακτηριστικό με τιμή κειμένου.
// Ορίστε τον τύπο ProjDurConv σε εκτεταμένο χαρακτηριστικό με τιμή διάρκειας και εκτυπώστε την τιμή του.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// Ορίστε τον τύπο ProjDurConv σε εκτεταμένο χαρακτηριστικό με τιμή κειμένου και εκτυπώστε την τιμή του.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// Ορίστε τον τύπο Second και εκτυπώστε την τιμή του εκτεταμένου χαρακτηριστικού.
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// Ορίστε τον τύπο Weekday και εκτυπώστε την τιμή του εκτεταμένου χαρακτηριστικού.
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### Δείτε επίσης

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


