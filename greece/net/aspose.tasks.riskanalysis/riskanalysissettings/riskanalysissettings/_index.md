---
title: "RiskAnalysisSettings.RiskAnalysisSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής RiskAnalysisSettings. Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης RiskAnalysisSettings"
type: docs
weight: 10
url: /el/net/aspose.tasks.riskanalysis/riskanalysissettings/riskanalysissettings/
---
## RiskAnalysisSettings constructor

Αρχικοποιεί ένα νέο στιγμιότυπο της κλάσης [`RiskAnalysisSettings`](../).

```csharp
public RiskAnalysisSettings()
```

## Παραδείγματα

Δείχνει πώς να προετοιμάσετε τις ρυθμίσεις ανάλυσης κινδύνου για προσομοιώσεις Monte Carlo.

```csharp
var riskAnalysisSettings = new RiskAnalysisSettings();

// Ορίστε τον αριθμό επαναλήψεων για την προσομοίωση Monte Carlo (η προεπιλεγμένη τιμή είναι 100).
riskAnalysisSettings.IterationsCount = 200;

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task = project.RootTask.Children.GetById(17);

// Αρχικοποιήστε ένα πρότυπο κινδύνου
var pattern = new RiskPattern(task);

// Επιλέξτε τύπο κατανομής για τη γεννήτρια τυχαίων αριθμών ώστε να δημιουργεί πιθανές τιμές (προς το παρόν υποστηρίζονται μόνο δύο τύποι, δηλαδή κανονική και ομοιόμορφη)
// Για περισσότερες λεπτομέρειες δείτε εδώ: https://en.wikipedia.org/wiki/Normal_distribution)
pattern.Distribution = ProbabilityDistributionType.Normal;

// Ορίστε το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο καλύτερο δυνατό σενάριο έργου 
// Η προεπιλεγμένη τιμή είναι 75, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η αισιόδοξη διάρκεια θα είναι 3 ημέρες
pattern.Optimistic = 70;

// Ορίστε το ποσοστό της πιο πιθανής διάρκειας εργασίας που μπορεί να συμβεί στο χειρότερο δυνατό σενάριο έργου 
// Η προεπιλεγμένη τιμή είναι 125, που σημαίνει ότι εάν η εκτιμώμενη καθορισμένη διάρκεια εργασίας είναι 4 ημέρες, τότε η απαισιόδοξη διάρκεια θα είναι 5 ημέρες.
pattern.Pessimistic = 130;

// Ορίστε ένα επίπεδο εμπιστοσύνης που αντιστοιχεί στο ποσοστό του χρόνου που οι πραγματικές τιμές θα βρίσκονται μεταξύ των αισιόδοξων και απαισιόδοξων εκτιμήσεων. 
// Μπορείτε να το θεωρήσετε ως μια τιμή τυπικής απόκλισης: όσο πιο αβέβαιοι είστε για τις εκτιμήσεις σας, τόσο μεγαλύτερη είναι η τιμή τυπικής απόκλισης που χρησιμοποιείται στη γεννήτρια τυχαίων αριθμών.
pattern.ConfidenceLevel = ConfidenceLevel.CL75;

riskAnalysisSettings.Patterns.Add(pattern);

var analyzer = new RiskAnalyzer(riskAnalysisSettings);
var analysisResult = analyzer.Analyze(project);
var rootEarlyFinish = analysisResult.GetRiskItems(RiskItemType.EarlyFinish).Get(project.RootTask);

Console.WriteLine("Expected value: {0}", rootEarlyFinish.ExpectedValue);
Console.WriteLine("StandardDeviation: {0}", rootEarlyFinish.StandardDeviation);
Console.WriteLine("10% Percentile: {0}", rootEarlyFinish.GetPercentile(10));
Console.WriteLine("50% Percentile: {0}", rootEarlyFinish.GetPercentile(50));
Console.WriteLine("90% Percentile: {0}", rootEarlyFinish.GetPercentile(90));
Console.WriteLine("Minimum: {0}", rootEarlyFinish.Minimum);
Console.WriteLine("Maximum: {0}", rootEarlyFinish.Maximum);

analysisResult.SaveReport(OutDir + "AnalysisReport_out.pdf");
```

### Δείτε επίσης

* class [RiskAnalysisSettings](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysissettings/)
* assembly [Aspose.Tasks](../../../)


