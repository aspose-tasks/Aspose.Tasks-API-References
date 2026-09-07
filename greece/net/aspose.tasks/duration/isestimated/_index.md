---
title: "Duration.IsEstimated"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Duration. Λαμβάνει μια τιμή που υποδεικνύει εάν η μονάδα χρόνου είναι εκτιμημένη. Η σημαία που καθορίζει εάν αυτή η παρουσία Duration είναι εκτιμημένη"
type: docs
weight: 30
url: /el/net/aspose.tasks/duration/isestimated/
---
## Duration.IsEstimated property

Λαμβάνει μια τιμή που υποδεικνύει αν η μονάδα χρόνου είναι εκτιμώμενη. Η σημαία που καθορίζει αν αυτή η παρουσία Duration είναι εκτιμώμενη.

```csharp
public bool IsEstimated { get; }
```

## Παραδείγματα

Δείχνει πώς να αναλύσετε ένα κείμενο από ένα ειδικά μορφοποιημένο κείμενο.

```csharp
var project = new Project();

// παραδείγματα διάρκειών:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// όπου 1 - αριθμός στοιχείων (ημέρα, εβδομάδα κ.λπ), d - ημέρα (h - ώρα, w - εβδομάδα) ? - σημαία εκτίμησης, e - σημαία λήξης

// προσπαθήστε να αναλύσετε μια εκτιμώμενη διάρκεια
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// προσπαθήστε να αναλύσετε μια εκτιμώμενη διάρκεια
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


