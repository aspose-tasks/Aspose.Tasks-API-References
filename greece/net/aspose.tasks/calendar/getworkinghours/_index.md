---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Επιστρέφει WorkUnit, Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας για το καθορισμένο χρονικό διάστημα"
type: docs
weight: 220
url: /el/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

Επιστρέφει WorkUnit - Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας για το καθορισμένο χρονικό διάστημα.

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| έναρξη | DateTime | Ημερομηνία έναρξης του διαστήματος. |
| τελείωση | DateTime | Ημερομηνία λήξης του διαστήματος. |

### Τιμή Επιστροφής

Παράδειγμα της κλάσης [`WorkUnit`](../../workunit/) που περιέχει Έναρξη, Λήξη και Διάρκεια των ωρών εργασίας.

## Παραδείγματα

Δείχνει πώς να λάβετε τις ώρες εργασίας για συγκεκριμένες ημερομηνίες.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ώρες εργασίας για συγκεκριμένη ημερομηνία
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 ώρες θα εκτυπωθούν
Console.WriteLine(workUnit.WorkingHours);
```

### Δείτε επίσης

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

Επιστρέφει την ποσότητα των εργάσιμων ωρών στην καθορισμένη ημερομηνία.

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | Η ημερομηνία για την οποία θα ληφθούν οι ώρες εργασίας. |

### Τιμή Επιστροφής

Ώρες εργασίας στην καθορισμένη ημερομηνία.

## Παραδείγματα

Δείχνει πώς να λάβετε τις ώρες εργασίας για μια συγκεκριμένη ημερομηνία.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ώρες εργασίας για συγκεκριμένη ημερομηνία
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// Θα εκτυπωθούν 8 ώρες
Console.WriteLine(workingHours.Hours);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


