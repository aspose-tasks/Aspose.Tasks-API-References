---
title: "ICalendar.GetTaskFinishDateFromDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος ICalendar. Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από τα τμήματα της ημερομηνίας έναρξης και τη διάρκεια εργασίας."
type: docs
weight: 50
url: /el/net/aspose.tasks/icalendar/gettaskfinishdatefromduration/
---
## ICalendar.GetTaskFinishDateFromDuration method

Υπολογίζει την ημερομηνία και ώρα λήξης της εργασίας από την ημερομηνία έναρξής της, τα διαχωρισμένα μέρη και τη διάρκεια εργασίας.

```csharp
public DateTime GetTaskFinishDateFromDuration(Task task, TimeSpan duration)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| εργασία | Εργασία | Η εργασία για την οποία θα υπολογιστεί η ημερομηνία λήξης. |
| διάρκεια | TimeSpan | Η διάρκεια προς υπολογισμό. |

### Τιμή Επιστροφής

Η ημερομηνία λήξης της εργασίας για την δεδομένη ημερομηνία έναρξης και διάρκεια.

## Παρατηρήσεις

Επιστρέφει DateTime.MinValue εάν η εργασία είναι σύνοψη, null ή η ημερομηνία έναρξής της δεν έχει οριστεί.

### Δείτε επίσης

* class [Task](../../task/)
* interface [ICalendar](../)
* namespace [Aspose.Tasks](../../icalendar/)
* assembly [Aspose.Tasks](../../../)


