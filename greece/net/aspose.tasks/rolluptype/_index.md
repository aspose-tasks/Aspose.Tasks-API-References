---
title: "Απαρίθμηση RollupType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.RollupType. Καθορίζει τον τύπο συγκέντρωσης"
type: docs
weight: 1950
url: /el/net/aspose.tasks/rolluptype/
---
## RollupType enumeration

Καθορίζει τον τύπο συγκέντρωσης.

```csharp
public enum RollupType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Null | `0` | Δείχνει τύπο συγκέντρωσης Null. |
| Maximum | `1` | Δείχνει μέγιστο τύπο συγκέντρωσης. |
| Minimum | `2` | Δείχνει ελάχιστο τύπο συγκέντρωσης. |
| Count | `3` | Δείχνει τύπο συγκέντρωσης Count. |
| Sum | `4` | Δείχνει τύπο συγκέντρωσης Sum. |
| Average | `5` | Δείχνει τύπο συγκέντρωσης Average. |
| AverageFirstSublevel | `6` | Δείχνει τύπο συγκέντρωσης Average First Sublevel. |
| CountFirstSublevel | `7` | Δείχνει τύπο συγκέντρωσης Count First Sublevel. |
| CountNonsummaries | `8` | Δείχνει τύπο συγκέντρωσης Count Non-Summaries. |

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


