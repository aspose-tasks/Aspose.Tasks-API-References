---
title: "WorkingTime.WorkingTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "WorkingTime constructor. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης WorkingTime με ένα διάστημα με τις καθορισμένες ώρες έναρξης και λήξης"
type: docs
weight: 10
url: /el/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`WorkingTime`](../) με ένα διάστημα με τις καθορισμένες ώρες έναρξης και λήξης.

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromTime | DateTime | ώρα έναρξης διαστήματος |
| toTime | DateTime | ώρα λήξης διαστήματος |

## Παραδείγματα

Δείχνει πώς να εργαστείτε με πληροφορίες χρόνου εργασίας.

```csharp
public void WorkWithWorkingTime()
{
    var project = new Project();
    var calendar = CreateCalendar(project);
    project.Set(Prj.Calendar, calendar);

    Console.WriteLine("Work Week Number: " + calendar.WeekDays.Count);

    // Αυτά τα δεδομένα αφορούν το κουμπί "Λεπτομέρειες". Μπορείτε να ορίσετε ειδικούς χρόνους εργασίας για συγκεκριμένη ημέρα της εβδομάδας ή ακόμη και να την κάνετε μη εργάσιμη.
    List<WeekDay> weekDays = calendar.WeekDays.ToList();
    foreach (var day in weekDays)
    {
        Console.WriteLine(day.DayType.ToString());

        // Μπορείτε περαιτέρω να διασχίσετε τους χρόνους εργασίας και να τους εμφανίσετε.
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}

public static Calendar CreateCalendar(Project project)
{
    var calendar = project.Calendars.Add("MyCalendar", project.Calendars.GetByName("Standard"));
    var workingTimes = new List<WorkingTime>
                           {
                               new WorkingTime(new DateTime(1, 1, 1, 9, 0, 0), new DateTime(1, 1, 1, 12, 0, 0)),
                               new WorkingTime(new DateTime(1, 1, 1, 13, 0, 0), new DateTime(1, 1, 1, 18, 0, 0))
                           };

    calendar.WeekDays.Add(new WeekDay(DayType.Monday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Wednesday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Thursday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Friday, workingTimes));
    calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
    calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

    return calendar;
}
```

### Δείτε επίσης

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`WorkingTime`](../) με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromTime | TimeSpan | Η ώρα έναρξης του διαστήματος αναπαρίσταται από τη δομή TimeSpan. |
| toTime | TimeSpan | Η ώρα λήξης του διαστήματος αναπαρίσταται από τη δομή TimeSpan. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Όταν το toTime είναι μικρότερο ή ίσο με το όρισμα toTime ή όταν το διάστημα μεταξύ fromTime και toTime είναι μεγαλύτερο από 24 ώρες. |

## Παραδείγματα

Η υπερφόρτωση του WorkingTime ctor μπορεί να χρησιμοποιηθεί για την αρχικοποίηση της έναρξης και του τέλους του διαστήματος χρησιμοποιώντας TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### Δείτε επίσης

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`WorkingTime`](../) με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| fromHours | Int32 | Η ώρα έναρξης του διαστήματος αναπαρίσταται με ακέραιο αριθμό ωρών (0-24). |
| toHours | Int32 | Η ώρα λήξης του διαστήματος αναπαρίσταται με ακέραιο αριθμό ωρών (0-24). |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentException | Όταν το toTime είναι μικρότερο ή ίσο με το όρισμα toTime ή όταν το διάστημα μεταξύ fromTime και toTime είναι μεγαλύτερο από 24 ώρες. |

## Παραδείγματα

Η υπερφόρτωση του WorkingTime ctor μπορεί να χρησιμοποιηθεί για την αρχικοποίηση της έναρξης και του τέλους του διαστήματος χρησιμοποιώντας ολόκληρες ώρες:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

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


