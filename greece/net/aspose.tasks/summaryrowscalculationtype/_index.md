---
title: "Απαρίθμηση SummaryRowsCalculationType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.SummaryRowsCalculationType. Καθορίζει τον τύπο υπολογισμού της τιμής των προσαρμοσμένων χαρακτηριστικών για τις γραμμές σύνοψης."
type: docs
weight: 2310
url: /el/net/aspose.tasks/summaryrowscalculationtype/
---
## SummaryRowsCalculationType enumeration

Καθορίζει τον τύπο υπολογισμού της τιμής του προσαρμοσμένου χαρακτηριστικού για γραμμές σύνοψης.

```csharp
public enum SummaryRowsCalculationType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| None | `0` | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης δεν υπολογίζεται. |
| Rollup | `1` | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τη λειτουργία συγκέντρωσης που ορίζεται στο [`RollupType`](../extendedattributedefinition/rolluptype/). |
| UseFormula | `2` | Σημαίνει ότι η τιμή του προσαρμοσμένου χαρακτηριστικού για τις γραμμές σύνοψης υπολογίζεται χρησιμοποιώντας τον τύπο που ορίζεται στο [`Formula`](../extendedattributedefinition/formula/). |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


