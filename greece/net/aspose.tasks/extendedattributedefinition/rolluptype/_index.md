---
title: "ExtendedAttributeDefinition.RollupType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Λαμβάνει ή ορίζει τον τρόπο με τον οποίο υπολογίζονται τα rollups"
type: docs
weight: 230
url: /el/net/aspose.tasks/extendedattributedefinition/rolluptype/
---
## ExtendedAttributeDefinition.RollupType property

Λαμβάνει ή ορίζει τον τρόπο υπολογισμού των συγκεντρώσεων.

```csharp
public RollupType RollupType { get; set; }
```

## Παρατηρήσεις

Η εγγραφή υποστηρίζεται επί του παρόντος μόνο για μορφή Xml.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με τον τύπο υπολογισμού ενός εκτεταμένου ορισμού ιδιότητας.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 16, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// Δημιουργήστε ορισμό ιδιότητας με τύπο 'Formula' όπου οι τιμές για φύλλα εργασιών και συνοπτικές εργασίες υπολογίζονται με τύπο.
var calculation = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date5, null);
calculation.CalculationType = CalculationType.Formula;
calculation.SummaryRowsCalculationType = SummaryRowsCalculationType.UseFormula;
calculation.Formula = "[stARt]";
project.ExtendedAttributes.Add(calculation);

// Δημιουργήστε ορισμό ιδιότητας όπου οι τιμές για συνοπτικές εργασίες υπολογίζονται με τύπο συγκέντρωσης 'Average'.
var lookup = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Cost1, null);
lookup.SummaryRowsCalculationType = SummaryRowsCalculationType.Rollup;
lookup.RollupType = RollupType.Average;
project.ExtendedAttributes.Add(lookup);
```

### Δείτε επίσης

* enum [RollupType](../../rolluptype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


