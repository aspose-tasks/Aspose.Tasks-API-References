---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Calendar. Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο"
type: docs
weight: 260
url: /el/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

Καθορίζει εάν η καθορισμένη ημέρα είναι εργάσιμη ημέρα σύμφωνα με το ημερολόγιο.

```csharp
public bool IsDayWorking(DateTime dt)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| dt | DateTime | Η ημερομηνία για να ελέγξετε αν η ημέρα είναι εργάσιμη. |

### Τιμή Επιστροφής

Αληθές εάν η ημέρα είναι εργάσιμη.

## Παραδείγματα

Δείχνει πώς να υπολογίσετε τις εργάσιμες ώρες.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// Πρόσβαση στην εργασία με Id
var task = project.RootTask.Children.GetById(1);

// Πρόσβαση στο Calendar και τις ημερομηνίες έναρξης και λήξης του
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// Πρόσβαση στον πόρο και το ημερολόγιό του
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// Λήψη Διάρκειας σε Λεπτά
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// Λήψη Διάρκειας σε Ώρες
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// Λήψη Διάρκειας σε Ημέρες
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### Δείτε επίσης

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


