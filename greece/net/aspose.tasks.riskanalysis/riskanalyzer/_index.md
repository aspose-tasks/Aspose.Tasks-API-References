---
title: "Κλάση RiskAnalyzer"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.RiskAnalysis.RiskAnalyzer κλάση. Εκτελεί προσομοίωση Monte Carlo βάσει των καθορισμένων ρυθμίσεων ανάλυσης κινδύνου"
type: docs
weight: 1890
url: /el/net/aspose.tasks.riskanalysis/riskanalyzer/
---
## RiskAnalyzer class

Πραγματοποιεί προσομοίωση Monte Carlo βασισμένη στις καθορισμένες ρυθμίσεις ανάλυσης κινδύνου.

```csharp
public class RiskAnalyzer
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [RiskAnalyzer](riskanalyzer/)(RiskAnalysisSettings) | Αρχικοποιεί μια νέα παρουσία της κλάσης `RiskAnalyzer`. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Settings](../../aspose.tasks.riskanalysis/riskanalyzer/settings/) { get; set; } | Λαμβάνει ή ορίζει την παρουσία της κλάσης [`RiskAnalysisSettings`](../riskanalysissettings/) που ορίζει τις απαραίτητες ρυθμίσεις για την ανάλυση κινδύνου. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Analyze](../../aspose.tasks.riskanalysis/riskanalyzer/analyze/)(Project) | Πραγματοποιεί ανάλυση κινδύνου για το καθορισμένο έργο. Η ανάλυση βασίζεται σε προσομοίωση Monte Carlo και το αποτέλεσμα είναι μια παρουσία της κλάσης [`RiskAnalysisResult`](../riskanalysisresult/). |

## Παραδείγματα

Δείχνει πώς να ξεκινήσετε την ανάλυση κινδύνων χρησιμοποιώντας &lt;see cref="Aspose.Tasks.RiskAnalysis.RiskAnalysisSettings" /&gt;.

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
var earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

settings = new RiskAnalysisSettings
{
    IterationsCount = 300
};

// αλλάξτε τις ρυθμίσεις
analyzer.Settings = settings;

analysisResult = analyzer.Analyze(project);
earlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", earlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", earlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", earlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", earlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", earlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", earlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", earlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Δείτε επίσης

* namespace [Aspose.Tasks.RiskAnalysis](../../aspose.tasks.riskanalysis/)
* assembly [Aspose.Tasks](../../)


