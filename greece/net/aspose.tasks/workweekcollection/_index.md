---
title: "Κλάση WorkWeekCollection"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.WorkWeekCollection class. Αντιπροσωπεύει μια συλλογή αντικειμένων WorkWeek."
type: docs
weight: 3650
url: /el/net/aspose.tasks/workweekcollection/
---
## WorkWeekCollection class

Αντιπροσωπεύει μια συλλογή από [`WorkWeek`](../workweek/) αντικείμενα.

```csharp
public class WorkWeekCollection : IList<WorkWeek>
```

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [Count](../../aspose.tasks/workweekcollection/count/) { get; } | Επιστρέφει τον αριθμό των αντικειμένων που περιέχονται σε αυτό το αντικείμενο `WorkWeekCollection`. |
| [Item](../../aspose.tasks/workweekcollection/item/) { get; set; } | Επιστρέφει το στοιχείο στο καθορισμένο δείκτη. |
| [ParentCalendar](../../aspose.tasks/workweekcollection/parentcalendar/) { get; } | Επιστρέφει το γονικό ημερολόγιο. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [Add](../../aspose.tasks/workweekcollection/add/)(WorkWeek) | Προσθέτει το στιγμιότυπο WorkWeek σε αυτό το αντικείμενο συλλογής. |
| [GetEnumerator](../../aspose.tasks/workweekcollection/getenumerator/)() | Επιστρέφει έναν απαριθμητή για αυτή τη συλλογή. |
| [ToList](../../aspose.tasks/workweekcollection/tolist/)() | Μετατρέπει το αντικείμενο WorkWeekCollection σε λίστα από [`WorkWeek`](../workweek/) αντικείμενα. |

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

* class [WorkWeek](../workweek/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


