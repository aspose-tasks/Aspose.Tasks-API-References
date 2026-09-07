---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας"
type: docs
weight: 200
url: /el/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τελείωση | DateTime | Η καθορισμένη ημερομηνία λήξης. |
| διάρκεια | Διάρκεια | Η καθορισμένη διάρκεια. |

### Τιμή Επιστροφής

Υπολογισμένη ημερομηνία έναρξης.

## Παραδείγματα

Δείχνει πώς να λάβετε μια ημερομηνία έναρξης με βάση την ημερομηνία λήξης και τη διάρκεια.

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ημερομηνία έναρξης με ημερομηνία λήξης και διάρκεια
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 Απριλίου 2020 9:00 π.μ. θα εκτυπωθεί
Console.WriteLine(startDate);
```

### Δείτε επίσης

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

Επιστρέφει την ημερομηνία έναρξης βάσει της καθορισμένης ημερομηνίας λήξης και διάρκειας.

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| τελείωση | DateTime | Η καθορισμένη ημερομηνία λήξης. |
| διάρκεια | TimeSpan | Η καθορισμένη διάρκεια. |

### Τιμή Επιστροφής

Υπολογισμένη ημερομηνία έναρξης.

## Παραδείγματα

Δείχνει πώς να λάβετε μια ημερομηνία έναρξης με ημερομηνία λήξης και διάρκεια (ως χρονικό διάστημα).

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// λάβετε ημερομηνία έναρξης με ημερομηνία λήξης και διάρκεια
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 Απριλίου 2020 9:00 π.μ. θα εκτυπωθεί
Console.WriteLine(startDate);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


