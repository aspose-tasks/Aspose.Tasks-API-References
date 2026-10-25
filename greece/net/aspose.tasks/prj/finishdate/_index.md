---
title: "Prj.FinishDate"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η ημερομηνία λήξης ενός έργου"
type: docs
weight: 330
url: /el/net/aspose.tasks/prj/finishdate/
---
## Prj.FinishDate field

Η ημερομηνία λήξης ενός έργου.

```csharp
public static readonly Key<DateTime, PrjKey> FinishDate;
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
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


