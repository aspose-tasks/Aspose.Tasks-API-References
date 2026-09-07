---
title: "Κλάση RiskItemStatistics"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.RiskAnalysis.RiskItemStatistics κλάση. Αντιπροσωπεύει ένα στοιχείο που αποθηκεύει στατιστικά δεδομένα για την εργασία του αναλυόμενου έργου"
type: docs
weight: 1900
url: /el/net/aspose.tasks.riskanalysis/riskitemstatistics/
---
## RiskItemStatistics class

Αντιπροσωπεύει ένα στοιχείο που αποθηκεύει στατιστικά δεδομένα για την εργασία του αναλυθέντος έργου.

```csharp
public class RiskItemStatistics
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [ExpectedValue](../../aspose.tasks.riskanalysis/riskitemstatistics/expectedvalue/) { get; } | Λαμβάνει την αναμενόμενη τιμή του στοιχείου κινδύνου. |
| [ItemType](../../aspose.tasks.riskanalysis/riskitemstatistics/itemtype/) { get; } | Λαμβάνει μια παρουσία της αρίθμησης [`RiskItemType`](../riskitemtype/). |
| [Maximum](../../aspose.tasks.riskanalysis/riskitemstatistics/maximum/) { get; } | Λαμβάνει τη μέγιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo. |
| [Minimum](../../aspose.tasks.riskanalysis/riskitemstatistics/minimum/) { get; } | Λαμβάνει τη ελάχιστη τιμή που δημιουργήθηκε κατά τη διάρκεια της προσομοίωσης Monte Carlo. |
| [StandardDeviation](../../aspose.tasks.riskanalysis/riskitemstatistics/standarddeviation/) { get; } | Λαμβάνει την τυπική απόκλιση του στοιχείου κινδύνου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [GetPercentile](../../aspose.tasks.riskanalysis/riskitemstatistics/getpercentile/)(int) | Λαμβάνει μια τιμή κάτω από την οποία ένα καθορισμένο ποσοστό των παραγόμενων δειγμάτων πέφτει. |
| override [ToString](../../aspose.tasks.riskanalysis/riskitemstatistics/tostring/)() | Επιστρέφει σύντομη αναπαράσταση συμβολοσειράς ενός στοιχείου κινδύνου. Οι ακριβείς λεπτομέρειες της αναπαράστασης δεν έχουν οριστεί και ενδέχεται να αλλάξουν. |

## Παραδείγματα

Δείχνει πώς να υπολογίσετε στατιστικά των κινδύνων.

```csharp
var settings = new RiskAnalysisSettings
{
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Αρχικοποιήστε ένα πρότυπο κινδύνου
var pattern = new RiskPattern(task)
{
    // Επιλέξτε τύπο κατανομής για τη γεννήτρια τυχαίων αριθμών ώστε να δημιουργεί πιθανές τιμές (προς το παρόν υποστηρίζονται μόνο δύο τύποι, δηλαδή κανονική και ομοιόμορφη)
    // Για περισσότερες λεπτομέρειες δείτε εδώ: https://en.wikipedia.org/wiki/Normal_distribution)
    Distribution = ProbabilityDistributionType.Normal,

    // Ορίστε το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου 
    // Η προεπιλεγμένη τιμή είναι 75, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η αισιόδοξη διάρκεια θα είναι 3 ημέρες
    Optimistic = 70,

    // Ορίστε το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου 
    // Η προεπιλεγμένη τιμή είναι 125, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η απαισιόδοξη διάρκεια θα είναι 5 ημέρες.
    Pessimistic = 130,

    // Ορίστε ένα επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές τιμές θα βρίσκονται μεταξύ των αισιόδοξων και απαισιόδοξων εκτιμήσεων. 
    // Μπορείτε να το θεωρήσετε ως μια τιμή τυπικής απόκλισης: όσο πιο αβέβαιοι είστε για τις εκτιμήσεις σας, τόσο μεγαλύτερη είναι η τιμή τυπικής απόκλισης που χρησιμοποιείται στη γεννήτρια τυχαίων αριθμών.
    ConfidenceLevel = ConfidenceLevel.CL75
};
settings.Patterns.Add(pattern);

// Αναλύστε τους κινδύνους του έργου
var analyzer = new RiskAnalyzer(settings);
var analysisResult = analyzer.Analyze(project);
var statistics = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Short statistic: " + statistics);
Console.WriteLine();
Console.WriteLine("Statistic details: ");
Console.WriteLine("Item Type: {0}", statistics.ItemType);
Console.WriteLine("Expected value: {0}", statistics.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", statistics.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", statistics.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", statistics.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", statistics.GetPercentile(90));
Console.WriteLine("Minimum: {0}", statistics.Minimum);
Console.WriteLine("Maximum: {0}", statistics.Maximum);
```

### Δείτε επίσης

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


