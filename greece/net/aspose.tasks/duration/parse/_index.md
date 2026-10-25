---
title: "Duration.Parse"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Μετατρέπει τη συγκεκριμένη συμβολοσειρά στην παρουσία της δομής Duration."
type: docs
weight: 10
url: /el/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Μετατρέπει τη συγκεκριμένη συμβολοσειρά στην παρουσία της δομής [`Duration`](../).

```csharp
public static Duration Parse(Project p, string value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| p | Project | τη συγκεκριμένη παρουσία της κλάσης [`Project`](../../project/) για τη μετατροπή της διάρκειας. |
| value | String | τη συγκεκριμένη συμβολοσειρά για μετατροπή. |

### Τιμή Επιστροφής

Επιστρέφει την μετατρεπόμενη παρουσία της δομής [`Duration`](../).

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


