---
title: "Κλάση GraphicalIndicatorCriteriaValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.GraphicalIndicatorCriteriaValue. Αντιπροσωπεύει μια τιμή που χρησιμοποιείται στον έλεγχο συνθηκών των κριτηρίων γραφικών δεικτών"
type: docs
weight: 750
url: /el/net/aspose.tasks/graphicalindicatorcriteriavalue/
---
## GraphicalIndicatorCriteriaValue class

Αντιπροσωπεύει μια τιμή που χρησιμοποιείται στον έλεγχο συνθήκης των κριτηρίων των γραφικών δεικτών.

```csharp
public sealed class GraphicalIndicatorCriteriaValue
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_1)(bool) | Δημιουργεί ένα παράδειγμα της κλάσης GraphicalIndicatorCriteriaValue με σταθερή τιμή σημαίας (bool). |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_2)(DateTime) | Δημιουργεί ένα παράδειγμα της κλάσης GraphicalIndicatorCriteriaValue με σταθερή τιμή DateTime. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_3)(decimal) | Δημιουργεί ένα παράδειγμα της κλάσης GraphicalIndicatorCriteriaValue με σταθερή δεκαδική τιμή. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor)(Duration) | Δημιουργεί ένα παράδειγμα της κλάσης GraphicalIndicatorCriteriaValue με σταθερή τιμή Duration. |
| [GraphicalIndicatorCriteriaValue](graphicalindicatorcriteriavalue/#constructor_4)(string) | Δημιουργεί ένα παράδειγμα της κλάσης GraphicalIndicatorCriteriaValue με σταθερή τιμή συμβολοσειράς. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [IsFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/isfieldlink/) { get; } | Λαμβάνει εάν το τρέχον παράδειγμα είναι σύνδεσμος πεδίου (αντιπροσωπεύει μια τιμή ενός πεδίου). |
| [RawValue](../../aspose.tasks/graphicalindicatorcriteriavalue/rawvalue/) { get; } | Λαμβάνει τη βασική σταθερά της τιμής Field. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| static [CreateFieldLink](../../aspose.tasks/graphicalindicatorcriteriavalue/createfieldlink/)(Field) | Δημιουργεί μια παρουσία της κλάσης GraphicalIndicatorCriteriaValue που αντιπροσωπεύει την τιμή του καθορισμένου πεδίου του MS Project. |
| override [ToString](../../aspose.tasks/graphicalindicatorcriteriavalue/tostring/)() | Επιστρέφει μια συμβολοσειρά που αντιπροσωπεύει το τρέχον αντικείμενο. |

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


