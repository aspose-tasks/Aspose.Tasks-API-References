---
title: "ExtendedAttributeDefinition.GraphicalIndicator"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα ExtendedAttributeDefinition. Λαμβάνει ή ορίζει πληροφορίες γραφικών δεικτών που σχετίζονται με το εκτεταμένο χαρακτηριστικό. Εφαρμόσιμο στη μορφή MPP."
type: docs
weight: 160
url: /el/net/aspose.tasks/extendedattributedefinition/graphicalindicator/
---
## ExtendedAttributeDefinition.GraphicalIndicator property

Λαμβάνει ή ορίζει πληροφορίες γραφικών δεικτών που σχετίζονται με το εκτεταμένο χαρακτηριστικό. Εφαρμόσιμο στη μορφή MPP.

```csharp
public GraphicalIndicatorsInfo GraphicalIndicator { get; set; }
```

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

* class [GraphicalIndicatorsInfo](../../graphicalindicatorsinfo/)
* class [ExtendedAttributeDefinition](../)
* namespace [Aspose.Tasks](../../extendedattributedefinition/)
* assembly [Aspose.Tasks](../../../)


