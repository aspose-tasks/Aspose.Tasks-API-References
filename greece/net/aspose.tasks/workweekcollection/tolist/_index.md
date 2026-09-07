---
title: "WorkWeekCollection.ToList"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "WorkWeekCollection μέθοδος. Μετατρέπει το αντικείμενο WorkWeekCollection σε λίστα αντικειμένων WorkWeek"
type: docs
weight: 60
url: /el/net/aspose.tasks/workweekcollection/tolist/
---
## WorkWeekCollection.ToList method

Μετατρέπει το αντικείμενο WorkWeekCollection σε λίστα αντικειμένων [`WorkWeek`](../../workweek/).

```csharp
public List<WorkWeek> ToList()
```

### Τιμή Επιστροφής

Λίστα αντικειμένων [`WorkWeek`](../../workweek/).

## Παραδείγματα

Δείχνει πώς να δημιουργήσετε μια προσαρμοσμένη εβδομάδα εργασίας για ένα ημερολόγιο.

```csharp
var project = new Project();
var calendar = project.Calendars.Add("Standard");
Calendar.MakeStandardCalendar(calendar);

var item = new WorkWeek();
item.Name = "My Work Week";
item.FromDate = new DateTime(2020, 4, 13, 8, 0, 0);
item.ToDate = new DateTime(2020, 4, 17, 17, 0, 0);
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
item.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Friday));
item.WeekDays.Add(new WeekDay(DayType.Saturday));
item.WeekDays.Add(new WeekDay(DayType.Sunday));
calendar.WorkWeeks.Add(item);

Console.WriteLine("Work Weeks Count: " + calendar.WorkWeeks.Count);
foreach (var workWeek in calendar.WorkWeeks)
{
    // Εμφανίζει το όνομα της εβδομάδας εργασίας, το όνομα του γονικού ημερολογίου, τις ημερομηνίες από και έως
    Console.WriteLine("Name: " + workWeek.Name);
    Console.WriteLine("Parent calendar name: " + calendar.Name);
    Console.WriteLine("From Date: " + workWeek.FromDate);
    Console.WriteLine("To Date: " + workWeek.ToDate);
    Console.WriteLine();

    // Αυτά τα δεδομένα αφορούν το κουμπί "Λεπτομέρειες". Μπορείτε να ορίσετε ειδικούς χρόνους εργασίας για συγκεκριμένη ημέρα της εβδομάδας ή ακόμη και να την κάνετε μη εργάσιμη.
    List<WeekDay> weekDays = workWeek.WeekDays.ToList();
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

    Console.WriteLine();
}
```

### Δείτε επίσης

* class [WorkWeek](../../workweek/)
* class [WorkWeekCollection](../)
* namespace [Aspose.Tasks](../../workweekcollection/)
* assembly [Aspose.Tasks](../../../)


