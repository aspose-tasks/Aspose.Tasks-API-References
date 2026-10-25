---
title: "ExtendedAttributeDefinition.SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Επιστρέφει ή ορίζει τον τύπο υπολογισμού της τιμής των προσαρμοσμένων χαρακτηριστικών για τις γραμμές σύνοψης"
type: docs
weight: 260
url: /el/net/aspose.tasks/extendedattributedefinition/summaryrowscalculationtype/
---
## ExtendedAttributeDefinition.SummaryRowsCalculationType property

Λαμβάνει ή ορίζει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης.

```csharp
public SummaryRowsCalculationType SummaryRowsCalculationType { get; set; }
```

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

* enum [SummaryRowsCalculationType](../../summaryrowscalculationtype/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


