---
title: "Calendar.WeekDays"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα Calendar. Λαμβάνει το WeekDaysCollection για αυτό το ημερολόγιο. Η συλλογή των εργάσιμων ημερών που ορίζουν το ημερολόγιο."
type: docs
weight: 120
url: /el/net/aspose.tasks/calendar/weekdays/
---
## Calendar.WeekDays property

Λαμβάνει το WeekDaysCollection για αυτό το ημερολόγιο. Η συλλογή των εργάσιμων ημερών που ορίζει το ημερολόγιο.

```csharp
public WeekDayCollection WeekDays { get; }
```

## Παραδείγματα

Δείχνει πώς να ορίσετε ένα νέο ημερολόγιο, να προσθέσετε ημέρες της εβδομάδας σε αυτό και να ορίσετε ώρες εργασίας για τις ημέρες.

```csharp
var project = new Project();

// Ορίστε ένα ημερολόγιο
var calendar = project.Calendars.Add("Calendar1");

// Προσθέστε εργάσιμες ημέρες από τη Δευτέρα έως την Πέμπτη με προεπιλεγμένα ωράρια
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Tuesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));
calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// Ορίστε την Παρασκευή ως σύντομη εργάσιμη ημέρα
var weekDay = new WeekDay(DayType.Friday);

// Ορίζει χρόνο εργασίας. Μόνο το τμήμα ώρας του DateTime είναι σημαντικό.
var workingTime = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 16);
weekDay.WorkingTimes.Add(workingTime);
weekDay.WorkingTimes.Add(workingTime2);
weekDay.DayWorking = true;
calendar.WeekDays.Add(weekDay);

// εργασία με το έργο...
```

### Δείτε επίσης

* class [WeekDayCollection](../../weekdaycollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


