---
title: "Duration.op_Inequality"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 150
url: /el/net/aspose.tasks/duration/op_inequality/
---
## Duration Inequality operator

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public static bool operator !=(Duration a, Duration b)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| α | Διάρκεια | Η πρώτη διάρκεια. |
| β | Διάρκεια | Η δεύτερη διάρκεια. |

### Τιμή Επιστροφής

μια τιμή που υποδεικνύει εάν αυτή η παρουσία δεν είναι ίση με ένα καθορισμένο αντικείμενο

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα διάρκειας.

```csharp
var project = new Project();

var duration1 = project.GetDuration(1, TimeUnitType.Day);
var duration2 = project.GetDuration(1, TimeUnitType.Day);
var duration3 = project.GetDuration(1, TimeUnitType.Hour);

// η ισότητα της διάρκειας ελέγχεται σε σχέση με το υποκείμενο χρονικό διάστημα
Console.WriteLine("Duration 1: " + duration1.TimeSpan);
Console.WriteLine("Duration 2: " + duration2.TimeSpan);
Console.WriteLine("Duration 3: " + duration3.TimeSpan);
Console.WriteLine("Are durations 1 and 2 equal: " + duration1.Equals(duration2));
Console.WriteLine("Are durations 1 and 3 equal: " + duration1.Equals(duration3));
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


