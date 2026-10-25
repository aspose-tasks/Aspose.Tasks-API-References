---
title: "Duration.GetHashCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Επιστρέφει μια τιμή κωδικού κατακερματισμού για αυτό το αντικείμενο"
type: docs
weight: 90
url: /el/net/aspose.tasks/duration/gethashcode/
---
## Duration.GetHashCode method

Επιστρέφει μια τιμή κώδικα κατακερματισμού για αυτό το αντικείμενο.

```csharp
public override int GetHashCode()
```

### Τιμή Επιστροφής

επιστρέφει μια τιμή κωδικού κατακερματισμού για αυτήν την παρουσία duration.

## Παραδείγματα

Δείχνει πώς να λάβετε έναν κωδικό κατακερματισμού μιας διάρκειας.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// ο κωδικός κατακερματισμού ενός ημερολογίου βασίζεται στον τύπο μονάδας χρόνου και στην αρχική τιμή της διάρκειας
// οπότε οι επόμενοι κωδικοί κατακερματισμού είναι ίσοι
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 2 Hash Code: {0}", duration2.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration2.GetHashCode()));

// αλλά οι κωδικοί κατακερματισμού της διάρκειας 1 και 3 δεν είναι
Console.WriteLine("Duration 1 Hash Code: {0}", duration1.GetHashCode());
Console.WriteLine("Duration 3 Hash Code: {0}", duration3.GetHashCode());
Console.WriteLine("Are duration's hash codes of duration 1 and duration 2 equal: {0}", duration1.GetHashCode().Equals(duration3.GetHashCode()));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


