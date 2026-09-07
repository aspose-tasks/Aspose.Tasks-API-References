---
title: "Project.GetDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Λαμβάνει αντικείμενο Duration με τον καθορισμένο αριθμό μονάδων και την προεπιλεγμένη μορφή διάρκειας που ορίζεται στις ρυθμίσεις του έργου DurationFormat"
type: docs
weight: 1100
url: /el/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

Λαμβάνει το αντικείμενο [`Duration`](../../duration/) με τον καθορισμένο αριθμό μονάδων και την προεπιλεγμένη μορφή διάρκειας που ορίζεται στις ρυθμίσεις του έργου [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | Double | καθορισμένος αριθμός μονάδων. |

### Τιμή Επιστροφής

Αντικείμενο Duration.

## Παρατηρήσεις

Αυτή η μέθοδος πρέπει να χρησιμοποιείται προσεκτικά επειδή επιστρέφει διαφορετικές διάρκειες ανάλογα με τη ρύθμιση Project.DurationFormat. Για παράδειγμα, το GetWork(1.0) θα επιστρέψει 1 ώρα όταν το Project.DurationFormat είναι TimeUnitType.Hour ή 1 ημέρα εάν το Project.DurationFormat είναι TimeUnitType.Day.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια παρουσία &lt;see cref="Aspose.Tasks.Duration" /&gt; με την προεπιλεγμένη μορφή διάρκειας του έργου χρησιμοποιώντας μεθόδους κατασκευής έργου.

```csharp
var project = new Project();

// λάβετε μια διάρκεια με την προεπιλεγμένη μορφή του έργου.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### Δείτε επίσης

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

Λαμβάνει το αντικείμενο [`Duration`](../../duration/) με τον καθορισμένο αριθμό μονάδων [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | Double | καθορισμένος αριθμός μονάδων. |
| timeUnit | TimeUnitType | καθορισμένη τιμή TimeUnitType. |

### Τιμή Επιστροφής

Αντικείμενο Duration.

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια παρουσία &lt;see cref="Aspose.Tasks.Duration" /&gt; χρησιμοποιώντας μεθόδους κατασκευής έργου.

```csharp
var project = new Project();

// λάβετε μια διάρκεια με την προεπιλεγμένη μορφή του έργου.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### Δείτε επίσης

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

Λαμβάνει το αντικείμενο [`Duration`](../../duration/) με την καθορισμένη τιμή TimeSpan και την καθορισμένη τιμή [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| timeSpan | TimeSpan | καθορισμένη τιμή TimeSpan. |
| timeUnit | TimeUnitType | καθορισμένη τιμή TimeUnitType. |

### Τιμή Επιστροφής

Αντικείμενο Duration.

### Δείτε επίσης

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


