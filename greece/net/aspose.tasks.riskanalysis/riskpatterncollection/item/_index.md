---
title: "RiskPatternCollection.Item"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "RiskPatternCollection ιδιότητα. Λαμβάνει το στιγμιότυπο της κλάσης RiskPattern για την καθορισμένη εργασία"
type: docs
weight: 30
url: /el/net/aspose.tasks.riskanalysis/riskpatterncollection/item/
---
## RiskPatternCollection indexer

Λαμβάνει το στιγμιότυπο της κλάσης [`RiskPattern`](../../riskpattern/) για την καθορισμένη εργασία.

```csharp
public RiskPattern this[Task task] { get; }
```

| Παράμετρος | Περιγραφή |
| --- | --- |
| εργασία | την καθορισμένη εργασία. |

### Τιμή Επιστροφής

το μοτίβο για την καθορισμένη εργασία.

## Παραδείγματα

Δείχνει πώς να εργαστείτε με συλλογές προτύπων κινδύνου.

```csharp
var settings = new RiskAnalysisSettings
{
    // Ορίστε τον αριθμό επαναλήψεων για την προσομοίωση Monte Carlo (η προεπιλεγμένη τιμή είναι 100).
    IterationsCount = 200
};

var project = new Project(DataDir + "Software Development Plan-1.mpp");
var task1 = project.RootTask.Children.GetById(17);
var task2 = project.RootTask.Children.GetById(18);

// εφόσον το RiskPatternCollection δεν είναι μόνο για ανάγνωση
Console.WriteLine("Is pattern collection read-only?: " + settings.Patterns.IsReadOnly);

// μπορεί κανείς να προσθέσει νέα πρότυπα 
var pattern1 = new RiskPattern(task1)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 60,
    Pessimistic = 140,
    ConfidenceLevel = ConfidenceLevel.CL75
};
var pattern2 = new RiskPattern(task2)
{
    Distribution = ProbabilityDistributionType.Normal,
    Optimistic = 70,
    Pessimistic = 130,
    ConfidenceLevel = ConfidenceLevel.CL75
};

settings.Patterns.Add(pattern1);
settings.Patterns.Add(pattern2);

// επανάληψη πάνω στα προστιθέμενα πρότυπα
Console.WriteLine("Patterns count: " + settings.Patterns.Count);
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// επεξεργαστείτε το πρότυπο στη συλλογή χρησιμοποιώντας πρόσβαση με δείκτη
settings.Patterns[task1].Optimistic = 70;
settings.Patterns[task1].Pessimistic = 140;

// ελέγξτε τα πρότυπα μετά τις επεξεργασίες
Console.WriteLine("Print edited patterns: ");
foreach (var pattern in settings.Patterns)
{
    Console.WriteLine("Task: " + pattern.Task);
    Console.WriteLine("Distribution: " + pattern.Distribution);
    Console.WriteLine("Optimistic: " + pattern.Optimistic);
    Console.WriteLine("Pessimistic: " + pattern.Pessimistic);
    Console.WriteLine("Confidence Level: " + pattern.ConfidenceLevel);
    Console.WriteLine();
}

// μπορούμε να αφαιρέσουμε το πρότυπο
Console.WriteLine("Removing the first pattern...");
settings.Patterns.Remove(pattern1);

// ελέγξτε ότι το πρότυπο δεν βρίσκεται στη συλλογή
Console.WriteLine("Is collection contains the first pattern?: " + settings.Patterns.Contains(pattern1));

// μπορεί κανείς να εκκαθαρίσει τη συλλογή με δύο τρόπους

// αντιγράψτε τα πρότυπα στον πίνακα και διαγράψτε τα ένα-ένα
var patterns = new RiskPattern[settings.Patterns.Count];
settings.Patterns.CopyTo(patterns, 0);
foreach (var pattern in patterns)
{
    settings.Patterns.Remove(pattern);
}

// ή μπορεί κανείς να καθαρίσει εντελώς μια συλλογή προτύπων
settings.Patterns.Clear();
```

### Δείτε επίσης

* class [RiskPattern](../../riskpattern/)
* class [Task](../../../aspose.tasks/task/)
* class [RiskPatternCollection](../)
* namespace [Aspose.Tasks.RiskAnalysis](../../riskpatterncollection/)
* assembly [Aspose.Tasks](../../../)


