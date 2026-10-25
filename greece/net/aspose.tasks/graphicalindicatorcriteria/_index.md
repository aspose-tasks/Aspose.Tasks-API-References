---
title: "Κλάση GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.GraphicalIndicatorCriteria. Αντιπροσωπεύει ένα κριτήριο γραφικού δείκτη που σχετίζεται με μια εκτεταμένη ιδιότητα"
type: docs
weight: 730
url: /el/net/aspose.tasks/graphicalindicatorcriteria/
---
## GraphicalIndicatorCriteria class

Αντιπροσωπεύει ένα κριτήριο γραφικού δείκτη που σχετίζεται με μια εκτεταμένη ιδιότητα.

```csharp
public sealed class GraphicalIndicatorCriteria
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue) | Αρχικοποιεί ένα νέο αντικείμενο του τύπου `GraphicalIndicatorCriteria`. |
| [GraphicalIndicatorCriteria](graphicalindicatorcriteria/#constructor_1)(GraphicalIndicatorCriteriaType, FilterComparisonType, int, GraphicalIndicatorCriteriaValue, GraphicalIndicatorCriteriaValue) | Αρχικοποιεί ένα νέο αντικείμενο του τύπου `GraphicalIndicatorCriteria`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ImageIndex](../../aspose.tasks/graphicalindicatorcriteria/imageindex/) { get; } | Λαμβάνει τον δείκτη της εικόνας που θα εμφανιστεί όταν το πεδίο πληροί τα κριτήρια. |
| [RowType](../../aspose.tasks/graphicalindicatorcriteria/rowtype/) { get; } | Λαμβάνει την τιμή του enum [`GraphicalIndicatorCriteriaType`](../graphicalindicatorcriteriatype/) που υποδεικνύει για ποιες γραμμές εφαρμόζεται ο δείκτης. |
| [Test](../../aspose.tasks/graphicalindicatorcriteria/test/) { get; } | Λαμβάνει τον τύπο σύγκρισης που γίνεται μεταξύ της τιμής της εκτεταμένης ιδιότητας και των τιμών που λειτουργούν ως κριτήριο για την εφαρμογή του γραφικού δείκτη. [`FilterComparisonType`](../filtercomparisontype/) |
| [Value1](../../aspose.tasks/graphicalindicatorcriteria/value1/) { get; } | Λαμβάνει την τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού. |
| [Value2](../../aspose.tasks/graphicalindicatorcriteria/value2/) { get; } | Λαμβάνει τη δεύτερη τιμή που χρησιμοποιείται για τη δοκιμή της τιμής του εκτεταμένου χαρακτηριστικού σε περιπτώσεις τύπων σύγκρισης 'IsWithin' και 'IsNotWithin'. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteria/tostring/)() | Επιστρέφει την αναπαράσταση σε μορφή συμβολοσειράς της παρουσίας της κλάσης `GraphicalIndicatorCriteria`. |

## Παραδείγματα

Δείχνει πώς να ανακτήσετε πληροφορίες γραφικών δεικτών.

```csharp
Project project = new Project(DataDir + "graphical_indicators.mpp");

foreach (var ea in project.ExtendedAttributes)
{
    if (ea.GraphicalIndicator == null)
    {
        continue;
    }

    Console.WriteLine("GI for field '{0}':", ea.FieldName);

    foreach (var criterion in ea.GraphicalIndicator.Criteria)
    {
        Console.WriteLine("Row type: {0}", criterion.RowType);
        Console.WriteLine("Image index: {0}", criterion.ImageIndex);
        Console.Write(criterion.Test);
        if (criterion.Value1 != null)
        {
            Console.Write(" ");
            Console.Write(criterion.Value1.RawValue);
        }

        if (criterion.Value2 != null)
        {
            Console.Write(" ");
            Console.WriteLine(criterion.Value2.RawValue);
        }

        Console.WriteLine();
    }
}
```

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


