---
title: "Project.GlobalizationSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Project. Λαμβάνει ή ορίζει ρυθμίσεις παγκοσμιοποίησης ειδικές για γλώσσες του έργου"
type: docs
weight: 460
url: /el/net/aspose.tasks/project/globalizationsettings/
---
## Project.GlobalizationSettings property

Αποκτά ή ορίζει τις ρυθμίσεις παγκοσμιοποίησης (συγκεκριμένες για τη γλώσσα) του έργου.

```csharp
public GlobalizationSettings GlobalizationSettings { get; set; }
```

## Παρατηρήσεις

Ο συνιστώμενος τρόπος είναι η χρήση κυριολεκτικών ή μορφών ανεξάρτητων από την κουλτούρα σε όλο το έργο. Ωστόσο, εάν ένα έργο χρησιμοποιεί κυριολεκτικά εξειδικευμένα για την κουλτούρα, αυτή η κλάση μπορεί να χρησιμοποιηθεί για να βοηθήσει τη μηχανή υπολογισμού να αναλύσει αυτά τα κυριολεκτικά.

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

* class [GlobalizationSettings](../../globalizationsettings/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


