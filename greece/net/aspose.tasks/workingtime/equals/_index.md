---
title: "WorkingTime.Equals"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος WorkingTime. Ελέγχει αν τα αντικείμενα είναι ίσα"
type: docs
weight: 40
url: /el/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Ελέγχει αν τα αντικείμενα είναι ίσα.

```csharp
public override bool Equals(object obj)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| obj | Αντικείμενο | Δεύτερο αντικείμενο για σύγκριση. |

### Τιμή Επιστροφής

Αληθές αν τα αντικείμενα είναι ίσα, ψευδές διαφορετικά.

## Παραδείγματα

Δείχνει πώς να ελέγξετε την ισότητα του χρόνου εργασίας.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// Η ισότητα των ημερολογίων ελέγχεται σε σχέση με τις ημερομηνίες from και to του χρόνου εργασίας.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Δείτε επίσης

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


