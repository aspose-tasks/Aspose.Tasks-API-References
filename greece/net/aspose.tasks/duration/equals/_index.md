---
title: "Duration.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο"
type: docs
weight: 80
url: /el/net/aspose.tasks/duration/equals/
---
## Equals(Duration) {#equals}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public bool Equals(Duration other)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| άλλο | Διάρκεια | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

Επιστρέφει **True** εάν η άλλη παρουσία Duration έχει τις ίδιες τιμές TimeSpan και TimeUnit με αυτήν την παρουσία· διαφορετικά, **false**.

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

---

## Equals(object) {#equals_1}

Επιστρέφει μια τιμή που υποδεικνύει εάν αυτή η παρουσία είναι ίση με ένα καθορισμένο αντικείμενο.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Το αντικείμενο για σύγκριση με αυτήν την παρουσία. |

### Τιμή Επιστροφής

**True** if the specified object is a Duration that has the same TimeSpan and TimeUnit values as this instance; otherwise, **false**.

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


