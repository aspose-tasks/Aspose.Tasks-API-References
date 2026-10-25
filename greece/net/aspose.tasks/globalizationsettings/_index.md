---
title: "Κλάση GlobalizationSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.GlobalizationSettings. Αντιπροσωπεύει τις ρυθμίσεις παγκοσμιοποίησης του έργου."
type: docs
weight: 720
url: /el/net/aspose.tasks/globalizationsettings/
---
## GlobalizationSettings class

Αντιπροσωπεύει τις ρυθμίσεις παγκοσμιοποίησης του project.

```csharp
public class GlobalizationSettings
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GlobalizationSettings](globalizationsettings/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| virtual [FalseLiteral](../../aspose.tasks/globalizationsettings/falseliteral/) { get; } | Λαμβάνει μια συμβολοσειρά για το λεκτικό boolean 'false' που χρησιμοποιείται σε τύπο. |
| virtual [FormulaDateNA](../../aspose.tasks/globalizationsettings/formuladatena/) { get; } | Λαμβάνει το λεκτικό "NA" (κενή τιμή) που χρησιμοποιείται σε τύπο για πεδίο ημερομηνίας. |
| virtual [TrueLiteral](../../aspose.tasks/globalizationsettings/trueliteral/) { get; } | Λαμβάνει μια συμβολοσειρά για το λεκτικό boolean 'true' που χρησιμοποιείται σε έναν τύπο. |

## Παρατηρήσεις

Ο συνιστώμενος τρόπος είναι η χρήση λεκτικών ή μορφών ανεξάρτητων από τον πολιτισμό σε όλο το έργο. Ωστόσο, εάν ένα έργο χρησιμοποιεί λεκτικά ειδικά για τον πολιτισμό, αυτή η κλάση μπορεί να χρησιμοποιηθεί για να βοηθήσει τη μηχανή υπολογισμού τύπων να αναλύσει αυτά τα λεκτικά.

## Παραδείγματα

Δείχνει πώς να ορίσετε τις γλωσσικές ρυθμίσεις του έργου.

```csharp
var project = new Project();

var attribute = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number");
attribute.Formula = "IIf(ProjDateValue('n.a.')=[Date1];100;200)";

project.ExtendedAttributes.Add(attribute);

var task = project.RootTask.Children.Add("Task");

// Δημιουργία εκτεταμένου χαρακτηριστικού
var extendedAttribute = attribute.CreateExtendedAttribute();
task.ExtendedAttributes.Add(extendedAttribute);

var attributeDate = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, "Date");

task.ExtendedAttributes.Add(attributeDate.CreateExtendedAttribute(DateTime.MinValue));

Console.WriteLine(extendedAttribute.NumericValue);

project.GlobalizationSettings = new MyGlobalizationSettings();

Console.WriteLine(extendedAttribute.NumericValue);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


