---
title: "ExtendedAttribute.DateValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttribute. Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά με τύπους ημερομηνίας Date, Start, Finish."
type: docs
weight: 20
url: /el/net/aspose.tasks/extendedattribute/datevalue/
---
## ExtendedAttribute.DateValue property

Λαμβάνει ή ορίζει μια τιμή για χαρακτηριστικά με τύπους ημερομηνίας (Date, Start, Finish).

```csharp
public DateTime DateValue { get; set; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| InvalidOperationException | Εκτοπίζεται εάν η ιδιότητα [`AttributeDefinition`](../attributedefinition/) δεν έχει αρχικοποιηθεί ή το τρέχον χαρακτηριστικό δεν είναι χαρακτηριστικό ημερομηνίας. |

## Παραδείγματα

Δείχνει πώς να αλλάξετε τον ορισμό του χαρακτηριστικού του εκτεταμένου χαρακτηριστικού.

```csharp
var project = new Project();

// δημιουργήστε νέο ορισμό επεκτατικού χαρακτηριστικού εργασίας
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Cost, ExtendedAttributeTask.Cost1, string.Empty);

// Προσθέστε έναν τύπο στην ιδιότητα.
definition.Alias = "Difference between Cost and Actual Cost";
definition.Formula = "[Cost]-[Actual Cost]";

project.ExtendedAttributes.Add(definition);

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
task.Set(Tsk.Deadline, new DateTime(2020, 4, 22, 17, 0, 0));
task.Set(Tsk.Cost, 20);
task.Set(Tsk.ActualCost, 13);

// δημιουργήστε εκτεταμένη ιδιότητα
var extendedAttribute = definition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

Console.WriteLine("Before change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.NumericValue);

// Δημιουργήστε έναν νέο ορισμό ημερομηνίας εκτεταμένου χαρακτηριστικού
var newDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Date, ExtendedAttributeTask.Date1, string.Empty);

// Προσθέστε έναν τύπο στην ιδιότητα.
newDefinition.Alias = "Days from finish to deadline";
newDefinition.Formula = "[Deadline] - [Finish]";
project.ExtendedAttributes.Add(newDefinition);

extendedAttribute = newDefinition.CreateExtendedAttribute();

Console.WriteLine();
Console.WriteLine("After change:");
Console.WriteLine("Alias: " + definition.Alias);
Console.WriteLine("Field Id: " + extendedAttribute.FieldId);
Console.WriteLine("Value: " + extendedAttribute.DateValue.Day);
```

### Δείτε επίσης

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


