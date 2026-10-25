---
title: "Prj.ScheduleFromStart"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει εάν θα υπολογιστεί το χρονοδιάγραμμα του έργου προς τα εμπρός από την ημερομηνία έναρξης"
type: docs
weight: 630
url: /el/net/aspose.tasks/prj/schedulefromstart/
---
## Prj.ScheduleFromStart field

Καθορίζει εάν θα υπολογιστεί το χρονοδιάγραμμα του έργου προς τα εμπρός από την ημερομηνία έναρξης.

```csharp
public static readonly Key<NullableBool, PrjKey> ScheduleFromStart;
```

## Παραδείγματα

Δείχνει πώς να επαναπρογραμματίσετε το έργο από την ημερομηνία λήξης αντί για την ημερομηνία έναρξης.

```csharp
var project = new Project();
project.Set(Prj.ScheduleFromStart, false);
project.Set(Prj.FinishDate, new DateTime(2020, 1, 1));

// Τώρα όλες οι ημερομηνίες των εργασιών (Start, Finish, EarlyStart, EarlyFinish, LateStart, LateFinish) υπολογίζονται. Για να λάβουμε τη κρίσιμη διαδρομή πρέπει να υπολογίσουμε τα περιθώρια (μπορούν να κληθούν σε ξεχωριστό νήμα, αλλά μόνο μετά τον υπολογισμό όλων των πρώιμων/τελευταίων ημερομηνιών).
project.Recalculate();

foreach (var task in project.CriticalPath)
{
    Console.WriteLine(task.Get(Tsk.Id));
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


