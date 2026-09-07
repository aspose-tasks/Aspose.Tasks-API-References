---
title: "RiskAnalysisResult.SaveReport"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "RiskAnalysisResult μέθοδος. Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη ροή σε μορφή PDF"
type: docs
weight: 20
url: /el/net/aspose.tasks.riskanalysis/riskanalysisresult/savereport/
---
## SaveReport(Stream) {#savereport}

Αποθηκεύει την αναφορά ανάλυσης κινδύνου στη ροή σε μορφή PDF.

```csharp
public void SaveReport(Stream stream)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| ροή | Ροή | Η ροή στην οποία θα αποθηκευτεί η αναφορά ανάλυσης κινδύνου. |

## Παραδείγματα

Δείχνει πώς να υπολογίσετε στατιστικά των κινδύνων και να τα αποθηκεύσετε ως αναφορά PDF.

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

// αποθηκεύστε την ανάλυση ως αναφορά σε αρχείο με διαδρομή αρχείου
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// ή αποθηκεύστε την ανάλυση σε ροή
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Δείτε επίσης

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)

---

## SaveReport(string) {#savereport_1}

Αποθηκεύει την αναφορά ανάλυσης κινδύνου στην καθορισμένη διαδρομή αρχείου σε μορφή PDF.

```csharp
public void SaveReport(string fileName)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fileName | String | Το καθορισμένο όνομα αρχείου. |

## Παραδείγματα

Δείχνει πώς να υπολογίσετε στατιστικά των κινδύνων και να τα αποθηκεύσετε ως αναφορά PDF.

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

// αποθηκεύστε την ανάλυση ως αναφορά σε αρχείο με διαδρομή αρχείου
analysisResult.SaveReport(OutDir + "AnalysisResult_out.pdf");

// ή αποθηκεύστε την ανάλυση σε ροή
using (var stream = new FileStream(OutDir + "AnalysisResult_out1.pdf", FileMode.Create))
{
    analysisResult.SaveReport(stream);
}
```

### Δείτε επίσης

* class [RiskAnalysisResult](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskanalysisresult/)
* assembly [Aspose.Tasks](../../../)


