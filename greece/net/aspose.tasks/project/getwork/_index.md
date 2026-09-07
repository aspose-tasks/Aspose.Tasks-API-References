---
title: "Project.GetWork"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Λαμβάνει αντικείμενο Duration με την καθορισμένη τιμή Double και προεπιλεγμένη μορφή εργασίας"
type: docs
weight: 1130
url: /el/net/aspose.tasks/project/getwork/
---
## Project.GetWork method

Λαμβάνει αντικείμενο [`Duration`](../../duration/) με την καθορισμένη τιμή Double και προεπιλεγμένη μορφή εργασίας.

```csharp
public Duration GetWork(double val)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| val | Double | καθορισμένη τιμή double. |

### Τιμή Επιστροφής

Αντικείμενο Duration.

## Παρατηρήσεις

Αυτή η μέθοδος πρέπει να χρησιμοποιείται προσεκτικά επειδή επιστρέφει διαφορετικές διάρκειες ανάλογα με τη ρύθμιση Project.WorkFormat. Για παράδειγμα, το GetWork(1.0) θα επιστρέψει 1 ώρα όταν το Project.WorkFormat είναι TimeUnitType.Hour ή 1 ημέρα αν το Project.WorkFormat είναι TimeUnitType.Day.

## Παραδείγματα

Δείχνει πώς να λάβετε μια εργασία με προεπιλεγμένη μορφή εργασίας.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// δημιουργήστε μια τιμή εργασίας με την προεπιλεγμένη μορφή εργασίας του έργου
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Δείτε επίσης

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


