---
title: "Κλάση GraphicalIndicatorsInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.GraphicalIndicatorsInfo. Αντιπροσωπεύει έναν ορισμό γραφικών δεικτών που σχετίζεται με μια εκτεταμένη ιδιότητα"
type: docs
weight: 760
url: /el/net/aspose.tasks/graphicalindicatorsinfo/
---
## GraphicalIndicatorsInfo class

Αντιπροσωπεύει έναν ορισμό γραφικών δεικτών που σχετίζεται με μια εκτεταμένη ιδιότητα.

```csharp
public sealed class GraphicalIndicatorsInfo
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GraphicalIndicatorsInfo](graphicalindicatorsinfo/)() | Αρχικοποιεί μια νέα παρουσία του τύπου `GraphicalIndicatorsInfo`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Criteria](../../aspose.tasks/graphicalindicatorsinfo/criteria/) { get; } | Λαμβάνει μια λίστα κριτηρίων γραφικών δεικτών. |
| [ProjectSummaryInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/projectsummaryinheritfromnonsummaryrows/) { get; set; } | Λαμβάνει ή ορίζει τη σημαία που υποδεικνύει εάν η γραμμή σύνοψης του έργου κληρονομεί κριτήρια από τις γραμμές σύνοψης. |
| [ShowDataValuesInTooltip](../../aspose.tasks/graphicalindicatorsinfo/showdatavaluesintooltip/) { get; set; } | Λαμβάνει ή ορίζει τη σημαία που υποδεικνύει εάν οι τιμές δεδομένων για το πεδίο πρέπει να εμφανίζονται σε υποδείξεις. |
| [SummaryRowsInheritFromNonSummaryRows](../../aspose.tasks/graphicalindicatorsinfo/summaryrowsinheritfromnonsummaryrows/) { get; set; } | Λαμβάνει ή ορίζει τη σημαία που υποδεικνύει εάν οι γραμμές σύνοψης κληρονομούν κριτήρια από τις μη-συνοπτικές γραμμές. |

## Παραδείγματα

Δείχνει πώς να ρυθμίσετε γραφικό δείκτη για ένα εκτεταμένο χαρακτηριστικό.

```csharp
Project project = new Project();

var def = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, "Number field");
project.ExtendedAttributes.Add(def);
def.GraphicalIndicator = new GraphicalIndicatorsInfo();

GraphicalIndicatorCriteria criteria1 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsLessThan,
    2,
    new GraphicalIndicatorCriteriaValue(100m));

// Το κριτήριο 'IsWithin' απαιτεί 2 τιμές.
GraphicalIndicatorCriteria criteria2 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsWithin,
    4,
    new GraphicalIndicatorCriteriaValue(101),
    new GraphicalIndicatorCriteriaValue(1000m));

// Το κριτήριο 'IsAnyValue' δεν απαιτεί τιμές.
GraphicalIndicatorCriteria criteria3 = new GraphicalIndicatorCriteria(
    GraphicalIndicatorCriteriaType.SummaryRows,
    FilterComparisonType.IsAnyValue,
    4,
    null);

def.GraphicalIndicator.Criteria.Add(criteria1);
def.GraphicalIndicator.Criteria.Add(criteria2);
def.GraphicalIndicator.Criteria.Add(criteria3);

def.GraphicalIndicator.ProjectSummaryInheritFromNonSummaryRows = true;
def.GraphicalIndicator.SummaryRowsInheritFromNonSummaryRows = true;
def.GraphicalIndicator.ShowDataValuesInTooltip = false;

project.Save(OutDir + "CreateGraphicalIndicators_out.mpp", SaveFileFormat.Mpp);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


