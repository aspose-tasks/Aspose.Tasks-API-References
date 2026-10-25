---
title: "Κλάση WorkingTime"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.WorkingTime. Αντιπροσωπεύει έναν χρόνο εργασίας κατά τη διάρκεια μιας εργάσιμης ημέρας."
type: docs
weight: 3660
url: /el/net/aspose.tasks/workingtime/
---
## WorkingTime class

Αντιπροσωπεύει έναν χρόνο εργασίας κατά τη διάρκεια μιας ημέρας της εβδομάδας.

```csharp
public class WorkingTime
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [WorkingTime](workingtime/#constructor_1)(DateTime, DateTime) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WorkingTime` με ένα διάστημα με τις καθορισμένες ώρες έναρξης και λήξης. |
| [WorkingTime](workingtime/#constructor)(int, int) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WorkingTime` με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης. |
| [WorkingTime](workingtime/#constructor_2)(TimeSpan, TimeSpan) | Αρχικοποιεί μια νέα παρουσία της κλάσης `WorkingTime` με ένα στοιχείο διαστήματος με τις καθορισμένες ώρες έναρξης και λήξης. |

## Ιδιότητες

| Όνομα | Περιγραφή |
| --- | --- |
| [From](../../aspose.tasks/workingtime/from/) { get; } | Λαμβάνει την αρχή ενός χρόνου εργασίας. |
| [To](../../aspose.tasks/workingtime/to/) { get; } | Λαμβάνει το τέλος ενός χρόνου εργασίας. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| override [Equals](../../aspose.tasks/workingtime/equals/)(object) | Ελέγχει αν τα αντικείμενα είναι ίσα. |
| override [GetHashCode](../../aspose.tasks/workingtime/gethashcode/)() | Επιστρέφει μια τιμή κώδικα κατακερματισμού για την παρουσία της κλάσης `WorkingTime`. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


