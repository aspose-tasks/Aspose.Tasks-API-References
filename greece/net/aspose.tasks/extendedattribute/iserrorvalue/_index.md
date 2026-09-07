---
title: "ExtendedAttribute.IsErrorValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttribute. Λαμβάνει εάν ο υπολογισμός της τιμής των εκτεταμένων χαρακτηριστικών κατέληξε σε σφάλμα."
type: docs
weight: 60
url: /el/net/aspose.tasks/extendedattribute/iserrorvalue/
---
## ExtendedAttribute.IsErrorValue property

Λαμβάνει εάν ο υπολογισμός της τιμής του επεκτατικού χαρακτηριστικού οδήγησε σε σφάλμα.

```csharp
public bool IsErrorValue { get; }
```

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

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


